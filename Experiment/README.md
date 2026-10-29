# 🌐 MAD Experiment 12: Access Web Services Using HTTP Request

An Android application demonstrating asynchronous web service consumption using HTTP GET requests, Kotlin Coroutines, and JSON parsing.

## 🎯 Aim

To develop an Android application that sends an HTTP GET request to a RESTful web service, retrieves JSON data, parses the response, and displays the user's name, email address, and city using Kotlin Coroutines.

## 🛠️ Technologies Used

- 💻 **Language:** Kotlin
- 📱 **IDE:** Android Studio
- 🌐 **Networking:** Java URL API
- ⚡ **Asynchronous Processing:** Kotlin Coroutines
- 🔄 **Thread Management:** Dispatchers.IO and Dispatchers.Main
- 📦 **Data Format:** JSON
- 🔗 **API:** JSONPlaceholder
- 🎨 **UI:** Android XML Layouts

## ✨ Features

- 🌐 Fetches user details from a RESTful web service using an HTTP GET request.
- ⚡ Performs network operations asynchronously using Kotlin Coroutines.
- 📄 Parses JSON responses using `JSONObject`.
- 👤 Displays the user's name, email address, and city.
- ⚠️ Handles network errors without crashing the application.
- 📱 Provides a simple Android user interface.

## 🔗 API Endpoint

The application uses the following public REST API:

https://jsonplaceholder.typicode.com/users/1

The API returns user information in JSON format, including the name, email, and address.

## 📂 Project Structure

```text
WebServiceHttpApp/
├── app/
│   ├── src/
│   │   └── main/
│   │       ├── AndroidManifest.xml
│   │       ├── java/com/example/webservicehttpapp/
│   │       │   └── MainActivity.kt
│   │       └── res/
│   │           └── layout/
│   │               └── activity_main.xml
│   └── build.gradle.kts
├── build.gradle.kts
├── settings.gradle.kts
└── README.md
```

## ⚙️ Implementation Details

### 1. 🌐 Internet Permission

Internet access is enabled by adding the following permission to `AndroidManifest.xml`:

```xml
<uses-permission android:name="android.permission.INTERNET" />
```

### 2. ⚡ Kotlin Coroutines

Kotlin Coroutines perform network operations in the background using `Dispatchers.IO`, while `Dispatchers.Main` updates the user interface safely.

### 3. 📄 JSON Parsing

The application uses `JSONObject` to extract the following information from the API response:

- **Name:** User's full name
- **Email:** User's email address
- **City:** User's city from the address object

### 4. 📦 Required Dependency

The following dependency is added to the app-level `build.gradle.kts` file:

```kotlin
implementation("org.jetbrains.kotlinx:kotlinx-coroutines-android:1.10.2")
```

## 🧪 Test Cases

| Test Case | Action | Expected Output |
|---|---|---|
| Initial Screen | Launch the application | Fetch button and result area are displayed |
| Successful Request | Tap the Fetch Web Data button with internet access | Name, email, and city are displayed |
| Network Error | Disable internet and tap the button | An error message is displayed without crashing |

## 📸 Screenshots

### 🏠 Initial Application Interface

<img width="526" height="1134" alt="InitialApplicationInterface" src="https://github.com/user-attachments/assets/dfa9e5ab-1ffa-4e7d-9250-38a3508aabeb" />


### 📊 Web Service Response

<img width="593" height="1021" alt="google-maps-location" src="https://github.com/user-attachments/assets/5626fad2-8d0c-43ba-8f60-41b3ff26a178" />



## ✅ Result

The Android application successfully demonstrates asynchronous HTTP GET requests to a RESTful web service using Kotlin Coroutines. The JSON response is parsed using `JSONObject`, and the retrieved user details are displayed on the screen. Network errors are handled appropriately without blocking the main UI thread.

## 👩‍💻 Author

**25MCAR0101 – Komal Gupta**

