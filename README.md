# Splash Screen Implementation for Android, iOS, Android 12, and Dark/Light Mode

This repository demonstrates how to implement a **custom splash screen** in a Flutter app that supports both **Dark Mode** and **Light Mode**, as well as compatibility with **Android 12** and **iOS**. The implementation uses the [`flutter_native_splash`](https://pub.dev/packages/flutter_native_splash) package to create a native splash screen experience.

## Features:
- **Dynamic Splash Screen**: Displays different splash screen images based on the system theme (Dark Mode or Light Mode).
- **Android 12 Support**: Fully compatible with Android 12's splash screen API.
- **iOS Support**: Works seamlessly on iOS devices.
- **Customizable**: Easy to customize for your app's branding.

## Screenshots:
- **Light Mode Splash Screen**:  
  ![Light Mode Splash Screen](screenshots/splash_light.png)  
- **Dark Mode Splash Screen**:  
  ![Dark Mode Splash Screen](screenshots/splash_dark.png)  

## How It Works:
1. **`flutter_native_splash` Package**:  
   The [`flutter_native_splash`](https://pub.dev/packages/flutter_native_splash) package is used to generate native splash screens for both Android and iOS. It ensures a smooth transition from the splash screen to the app.

2. **Dark Mode and Light Mode**:  
   The app detects the system theme (Dark or Light) and displays the appropriate splash screen image. This is achieved by dynamically switching between two images (`splash_light.png` and `splash_dark.png`) based on the theme.

3. **Android 12 Compatibility**:  
   The splash screen is optimized for Android 12's new splash screen API, ensuring a modern and consistent user experience.

4. **iOS Compatibility**:  
   The splash screen works seamlessly on iOS devices, providing a native look and feel.

## How to Use:
1. Add the `flutter_native_splash` package to your `pubspec.yaml` file.
2. Place your splash screen images (`splash_light.png` and `splash_dark.png`) in the `assets` folder.
3. Configure the `flutter_native_splash` settings in your `pubspec.yaml` file.
4. Use the provided code to dynamically switch between splash screen images based on the system theme.

## Example Configuration:
```yaml
flutter_native_splash:
  image: assets/splash_light.png  # Default image for Light Mode
  color: "#FFFFFF"                # Background color for Light Mode
  dark_image: assets/splash_dark.png  # Image for Dark Mode
  dark_color: "#121212"           # Background color for Dark Mode
