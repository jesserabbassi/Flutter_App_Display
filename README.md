# 📱 Flutter WebView App – Ooredoo App Wrapper

## 🚀 Overview

This project is a **Flutter mobile application** that wraps a deployed web application using a **WebView**.
It allows users to access the web app as a native Android app (APK).

---

## 🧰 Tech Stack

* **Flutter** – Mobile app framework
* **Dart** – Programming language
* **WebView (webview_flutter)** – To display the web app
* **Android Studio** – For building and testing APK

---

## 🌐 Web App

The mobile app loads the deployed web application:

👉 https://ooredoo-app-1.onrender.com/

---

## 📦 Features

* Displays the web app inside a native mobile app
* Supports JavaScript execution
* Works on real Android devices
* Simple and lightweight

---

## ⚙️ Installation & Setup

### 1. Clone the repository

```bash
git clone https://github.com/jesserabbassi/Flutter_App_Display.git
cd Flutter_App_Display
```

---

### 2. Install dependencies

```bash
flutter pub get
```

---

### 3. Run the app (recommended first)

```bash
flutter run
```

---

### 4. Build APK

```bash
flutter build apk
```

APK location:

```
build/app/outputs/flutter-apk/app-release.apk
```

---

## 📱 Installing on Phone

1. Transfer the APK to your Android device
2. Enable **"Install unknown apps"**
3. Install the APK

---

## ⚠️ Important Configuration

### Internet Permission (REQUIRED)

Make sure this is added in:

```
android/app/src/main/AndroidManifest.xml
```

```xml
<uses-permission android:name="android.permission.INTERNET"/>
```

Without this, the app will not load any website.

---

### Minimum SDK

Ensure:

```kotlin
minSdk = 21
```

---

## 🐛 Known Issues

* WebView may behave differently from a normal browser
* Some websites with authentication or redirects may need adjustments
* Requires stable internet connection

---

## 🧠 Lessons Learned

* Emulator ≠ real device behavior
* WebView requires proper Android permissions
* Deployment URLs must be public (not localhost)

---

## 📌 Future Improvements

* Add splash screen
* Add loading indicator
* Handle offline mode
* Improve UI (remove default AppBar, full screen mode)

---

## 👨‍💻 Author

Developed by **Jesser Abbassi**

---

## ⭐ Support

If you like this project, consider giving it a ⭐ on GitHub!
