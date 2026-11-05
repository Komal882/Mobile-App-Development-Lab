# 🗺️ DayPlanner – Sightseeing To-Do & Best Route Planner

An Android application that helps travellers organize sightseeing locations, manage their travel itinerary, and discover an optimized route with nearby food and rest stops using Google Maps APIs.

## 📌 Project Overview

DayPlanner is an Android-based travel planning application developed using Kotlin and XML in Android Studio. It allows users to create a personalized sightseeing list, visualize locations on Google Maps, mark visited places, and generate an optimized travel route.

The application integrates Google Maps, Directions API, and Places API to provide an interactive trip-planning experience.

## ✨ Key Features

### 1. Sightseeing To-Do List
- Add sightseeing places manually.
- Delete unwanted locations.
- Mark places as completed using checkboxes.
- Prevent blank and duplicate entries.
- Display place names, categories, and geographical coordinates.

### 2. Google Maps Integration
- Display sightseeing locations using map markers.
- Different marker colors for sightseeing, food, and rest stops.
- Add new locations using long-press on the map.
- View location details by tapping markers.
- Synchronize map markers with the To-Do list.

### 3. Best Route Planner
- Generate an optimized visiting sequence using Google Directions API.
- Use waypoint optimization to determine the visiting order.
- Decode Google Maps overview polyline data.
- Display the route on Google Maps.
- Automatically adjust map zoom to show the complete itinerary.

### 4. Automatic Food & Rest Stops
- Find nearby restaurants using Google Places API.
- Automatically insert a food stop near the middle of the itinerary.
- Find nearby hotels or lounges for rest stops.
- Prevent duplicate stop insertion.

### 5. Adaptive User Interface
- **Portrait Mode:** Separate tabs for To-Do List and Map View.
- **Landscape Mode:** Side-by-side layout displaying the list and map.
- Responsive interface with improved spacing and readable text.
## 📱 Application Screenshots


# 🗺️ DayPlanner – Sightseeing To-Do & Best Route Planner

An Android application that helps travellers organize sightseeing locations, manage their travel itinerary, and discover an optimized route with nearby food and rest stops using Google Maps APIs.

## 📱 Application Screenshots

### Google Maps – Planned Route
![DayPlanner Map View](screenshots/map-view.png)

### Sightseeing To-Do List
![DayPlanner To-Do List](screenshots/todo-list.png)

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| Kotlin | Android application development |
| XML | UI design and layouts |
| Android Studio | Development environment |
| Google Maps SDK | Interactive map integration |
| Google Directions API | Route optimization |
| Google Places API | Nearby restaurant and hotel search |
| Android ListView | Display sightseeing locations |
| Custom ArrayAdapter | Manage list items |
| Android Location APIs | Location handling |
| Gradle | Project configuration |


## 🏗️ Application Architecture

The application is organized around the following components:

- **MainActivity.kt:** Main application logic, UI interactions, map integration, and route planning.
- **PlaceItem.kt:** Data model representing individual sightseeing, food, and rest locations.
- **PlaceAdapter.kt:** Custom adapter for displaying and managing To-Do list items.
- **MapServices.kt:** Helper class for Directions API requests, Places API requests, and polyline decoding.
- **activity_main.xml:** Main portrait layout.
- **layout-land/activity_main.xml:** Landscape layout.
- **item_place.xml:** Custom layout for individual place list items.

## 🔑 API Configuration

This project requires a Google Maps Platform API key.

Enable the following APIs in Google Cloud Console:

1. Maps SDK for Android
2. Directions API
3. Places API

### Configure API Key

1. Create a Google Maps Platform API key.
2. Open the project's `local.properties` file.
3. Add the following configuration:

```properties
MAPS_API_KEY=YOUR_GOOGLE_MAPS_API_KEY
```

4. Sync the Gradle project.
5. Ensure the API key is correctly injected through Gradle configuration and AndroidManifest.xml.

**Security Note:** Never upload your actual API key or `local.properties` file to GitHub. Restrict API key usage through Google Cloud Console.

## 🚀 Installation & Setup

### Prerequisites
- Android Studio
- Android SDK
- Kotlin support
- Google Maps Platform API key
- Android device or emulator

### Steps

1. Clone the repository:

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

2. Open the project in Android Studio.

3. Configure your Google Maps API key in `local.properties`.

4. Sync Gradle files.

5. Connect an Android device or start an emulator.

6. Build and run the application.

## 🧪 Testing

The following functionalities are included in the application testing:

- Adding and deleting sightseeing locations.
- Marking locations as completed.
- Preventing duplicate entries.
- Adding locations through map long-press.
- Displaying and synchronizing map markers.
- Generating a route using Directions API.
- Inserting nearby food and rest stops.
- Testing portrait and landscape layouts.
- Handling API and network failures.

## 🎯 Learning Outcomes

Through this project, I gained practical experience in:

- Android application development using Kotlin.
- Designing user interfaces using XML.
- Integrating Google Maps SDK.
- Working with external REST APIs.
- Handling geographical coordinates and map markers.
- Implementing route optimization.
- Managing dynamic ListView data.
- Designing adaptive Android layouts.
- Handling API responses and errors.

## 🔮 Future Enhancements

- Save travel plans permanently using Room Database.
- Add user authentication and personalized profiles.
- Display estimated travel time and distance.
- Add live GPS navigation.
- Allow users to share their travel itineraries.
- Add search suggestions and location autocomplete.

## 👩‍💻 Author

**Komal Gupta**

Android Application Development Project

---

⭐ If you find this project interesting, consider giving the repository a star!
