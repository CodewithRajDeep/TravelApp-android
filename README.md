# TravelApp Project: Android Application

## Overview
This project is an Android application designed to implement Google Maps, location services, image loading with Glide, and permission handling using Dexter. The application includes support for modern UI components and uses the latest Android libraries.

---

## Prerequisites

Ensure the following tools are installed on your system:

1. **Android Studio** (Latest stable version).
2. **JDK 11** or higher.
3. **Gradle** (comes with Android Studio).
4. **Git** (to clone the repository).

---

## Project Setup

Follow these steps to set up and run the project on your local system:

### 1. Clone the Repository
```bash
git clone <repository_url>
cd <repository_name>
```

Replace `<repository_url>` with the actual Git repository URL.

### 2. Open the Project in Android Studio
1. Launch Android Studio.
2. Click on **File > Open**.
3. Select the folder where you cloned the repository.
4. Let Android Studio sync and build the project automatically.

### 3. Configure SDKs
1. Go to **File > Project Structure > SDK Location**.
2. Ensure the **Android SDK** path is set correctly.
3. Make sure you have **API Level 34** (compileSdk) and **API Level 33** (targetSdk) installed.
4. Install additional dependencies if prompted.

### 4. Build the Project
Ensure Gradle builds the project correctly:
```bash
./gradlew build
```

Alternatively, click **Build > Rebuild Project** in Android Studio.

### 5. Run the Project on an Emulator or Device
1. Connect an Android device or start an emulator.
2. Ensure USB Debugging is enabled on your device (if using a physical device).
3. Click **Run > Run 'app'** or press **Shift + F10** in Android Studio.

### 6. Commands Summary
- **Clone the Repository:**
  ```bash
  git clone <repository_url>
  ```
- **Build the Project:**
  ```bash
  ./gradlew build
  ```
- **Run the Project:**
  ```bash
  ./gradlew installDebug
  ```

---

## Project Dependencies
The project uses the following libraries:

- **Glide**: Efficient image loading and caching.
  ```gradle
  implementation 'com.github.bumptech.glide:glide:4.11.0'
  ```
- **Google Play Services** (Maps and Location):
  ```gradle
  implementation 'com.google.android.gms:play-services-maps:19.0.0'
  implementation 'com.google.android.gms:play-services-location:21.3.0'
  ```
- **Dexter**: Runtime permissions handling.
  ```gradle
  implementation 'com.karumi:dexter:6.2.3'
  ```
- **Material Design Components**: UI/UX enhancements.
  ```gradle
  implementation 'com.google.android.material:material:1.12.0'
  ```
- **JUnit** and **Espresso**: For unit and UI testing.
  ```gradle
  testImplementation 'junit:junit:4.13.2'
  androidTestImplementation 'androidx.test.ext:junit:1.2.1'
  androidTestImplementation 'androidx.test.espresso:espresso-core:3.6.1'
  ```

---

## Important Notes

1. **Min SDK:** 24
2. **Target SDK:** 33
3. **Build Tools Version:** 34.0.0
4. **ProGuard:** Ensure ProGuard rules are set correctly for release builds.
5. **Permissions:**
   - Add necessary permissions for location and internet in `AndroidManifest.xml`:
     ```xml
     <uses-permission android:name="android.permission.ACCESS_FINE_LOCATION"/>
     <uses-permission android:name="android.permission.ACCESS_COARSE_LOCATION"/>
     <uses-permission android:name="android.permission.INTERNET"/>
     ```

---

## Troubleshooting

### Common Issues:
- **Gradle Sync Issues**: Ensure you have a stable internet connection and the correct Gradle version.
- **Device Not Recognized**: Check USB drivers or enable USB Debugging on your device.
- **Library Version Conflicts**: Update dependencies in the `build.gradle` file if necessary.

### Logs:
Use Android Studio's **Logcat** to debug runtime errors or crashes.

---

## Contribution

Feel free to fork this repository and contribute:
1. Create a feature branch.
2. Make your changes.
3. Push your changes and create a pull requests.

---

## License
This project is licensed under the [MIT License](LICENSE).

---

Thank you for using this project! If you encounter any issues, feel free to reach out.

