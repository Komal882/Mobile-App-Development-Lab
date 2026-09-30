# Experiment 08 – Implementing Menus and WebView in an Android Application

## 📌 Experiment Title

**Implementing Menus and WebView in an Android Application**

---

## 🎯 Objective

To develop an Android application that demonstrates the implementation of
**Options Menu, WebView, Image Grid, Local Media Selection, and Navigation**
within an Android application.

---

## 🛠️ Technologies Used

- Android Studio
- Kotlin
- XML
- Android SDK
- WebView
- Options Menu
- ImageView
- Grid Layout
- Local Media / Photo Picker

---

## 📱 Application Name

**Web & Media Explorer**

The application provides a simple interface for exploring web content and
media resources within an Android application.

---

## ✨ Features

### 1. Image Grid

The application displays different media items in a two-column grid.

Each item contains:

- Image/Media preview
- Category label
- Title
- Selection indicator
- More options menu

The Image Grid provides an organized way to display multiple media resources.

### 2. WebView

The application includes an integrated WebView for displaying web content
inside the Android application.

The WebView screen contains:

- Web Explorer header
- Home
- About
- Contact
- Offline local HTML content
- Explore Features section
- In-App WebView information

### 3. Options Menu

An options menu is available from the three-dot menu in the application
toolbar.

It provides additional actions for interacting with the application.

### 4. Photo Picker

The application demonstrates the Android photo/media selection interface
for accessing photos and media available on the device.

### 5. Bottom Navigation

The application provides navigation between:

- **Web View**
- **Image Grid**

---

## 🖥️ Application Screenshots

### 1. Image Grid

The Image Grid displays media resources in a two-column layout.

![Image Grid](screenshots/image_grid.png)

---

### 2. Photo Picker

The application can open the device's photo selection interface for
selecting media.

![Photo Picker](screenshots/photo_picker.png)

---

### 3. WebView

The WebView displays the local web content inside the Android application.

![WebView](screenshots/webview.png)

---

## 🧩 Main Components

| Component | Purpose |
|---|---|
| `MainActivity.kt` | Handles application logic and user interactions |
| `activity_main.xml` | Defines the main application UI |
| `main_menu.xml` | Defines the application options menu |
| `WebView` | Displays web content inside the application |
| `ImageView` | Displays media/images |
| `GridLayout` | Displays media items in a grid |
| Bottom Navigation | Switches between Web View and Image Grid |

---

## 🌐 WebView Implementation

The WebView is used to display web content directly inside the application.

The application supports local web content through the application's
HTML assets.

Example configuration:

```kotlin
webView.settings.javaScriptEnabled = true
webView.settings.domStorageEnabled = true
webView.webViewClient = WebViewClient()
