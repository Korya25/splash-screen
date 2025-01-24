# Splash Screen Implementation for Android, iOS, Android 12, and Dark/Light Mode

This repository demonstrates how to implement a **custom splash screen** in a Flutter app that supports both **Dark Mode** and **Light Mode**, as well as compatibility with **Android 12** and **iOS**. The implementation uses the [`flutter_native_splash`](https://pub.dev/packages/flutter_native_splash) package to create a native splash screen experience. Additionally, it includes **icons** and **animations** for a more engaging user experience.

## Features:
- **Dynamic Splash Screen**: Displays different splash screen images based on the system theme (Dark Mode or Light Mode).
- **Android 12 Support**: Fully compatible with Android 12's splash screen API.
- **iOS Support**: Works seamlessly on iOS devices.
- **Customizable**: Easy to customize for your app's branding.
- **Icons and Animations**: Includes icons and animations for a polished user experience.

## Screenshots:
| **Light Mode Splash Screen** | **Dark Mode Splash Screen** |
|------------------------------|-----------------------------|
| ![27d41fe9-e78d-414a-a05e-630bd624012a](https://github.com/user-attachments/assets/84b98157-8158-40c5-9076-954b7d808c96)| ![19fd7834-cff1-4ecf-a95c-739fcab7b3f9](https://github.com/user-attachments/assets/42449719-d70c-49ca-b073-6329db41b853)
 |


## How It Works:
1. **`flutter_native_splash` Package**:  
   The [`flutter_native_splash`](https://pub.dev/packages/flutter_native_splash) package is used to generate native splash screens for both Android and iOS. It ensures a smooth transition from the splash screen to the app.

2. **Dark Mode and Light Mode**:  
   The app detects the system theme (Dark or Light) and displays the appropriate splash screen image. This is achieved by dynamically switching between two images (`splash_light.png` and `splash_dark.png`) based on the theme.

3. **Icons and Animations**:  
   The splash screen includes a custom icon and an animation using the `lottie` package for a more engaging experience.

4. **Android 12 Compatibility**:  
   The splash screen is optimized for Android 12's new splash screen API, ensuring a modern and consistent user experience.

5. **iOS Compatibility**:  
   The splash screen works seamlessly on iOS devices, providing a native look and feel.

## How to Use:
1. Add the `flutter_native_splash` and `lottie` packages to your `pubspec.yaml` file.
2. Place your splash screen images (`splash_light.png` and `splash_dark.png`) and animation file (`animation.json`) in the `assets` folder.
3. Configure the `flutter_native_splash` settings in your `pubspec.yaml` file.
4. Use the provided code to dynamically switch between splash screen images and display animations based on the system theme.

## Example Configuration:
```yaml
flutter_native_splash:
  image: assets/splash_light.png  # Default image for Light Mode
  color: "#FFFFFF"                # Background color for Light Mode
  dark_image: assets/splash_dark.png  # Image for Dark Mode
  dark_color: "#121212"           # Background color for Dark Mode

dependencies:
  flutter:
    sdk: flutter
  lottie: ^2.7.0  # For animations
