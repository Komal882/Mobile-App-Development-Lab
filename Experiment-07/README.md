Experiment 07 – Adaptive Android Application with ListView and ImageView

📱 Experiment Title

Creating an Adaptive Android Application with ListView and ImageView

🎯 Objective

To develop an Android application using ListView and ImageView to display campus facilities in an interactive and user-friendly interface.

📝 Description

Campus Facilities is an Android application that displays a list of campus facilities with their images, names, and descriptions. When the user selects a facility, the application dynamically displays the corresponding image and details in the ImageView section below the list.

✨ Features

Custom ListView for displaying campus facilities

ImageView for facility images

Custom list-item layout using XML

Dynamic content update on item selection

Toast notification for selected facility

Clean and responsive user interface

Local image resources stored in res/drawable

🏫 Facilities Included

Facility

Description

Library

Books and study area

Computer Lab

Computers and practical sessions

Sports Complex

Indoor and outdoor sports

Cafeteria

Food and refreshments

Auditorium

Events and seminars

🛠️ Technologies Used

Kotlin

Android Studio

XML

ListView

ImageView

TextView

Toast

🔄 Application Flow

Launch the Campus Facilities application.

View the available facilities in the ListView.

Tap any facility.

The selected facility image is displayed below the list.

The facility name and description are updated dynamically.

A Toast message confirms the selected facility.

📸 Screenshots

1. Campus Facilities – Main Screen



2. Selected Facility – Dynamic ImageView



📂 Project Structure

AdaptiveListView/
│
├── app/
│   └── src/main/
│       ├── java/com/example/adaptivelistview/
│       │   └── MainActivity.kt
│       │
│       └── res/
│           ├── drawable/
│           │   ├── library.jpg
│           │   ├── computer_lab.jpg
│           │   ├── sports_complex.jpg
│           │   ├── cafeteria.jpg
│           │   └── auditorium.jpg
│           │
│           └── layout/
│               ├── activity_main.xml
│               └── item_facility.xml
│
└── README.md

🧩 Key Implementation

The application uses a custom ArrayAdapter to populate the ListView. Each Facility object contains a name, description, and drawable image resource.

When an item is clicked, the selected facility's image and information are updated dynamically in the ImageView and TextViews.

✅ Result

The application successfully demonstrates the implementation of an adaptive Android interface using ListView and ImageView, with dynamic image and content updates based on user selection.

Experiment: 07
Application: AdaptiveListView
Language: Kotlin
IDE: Android Studio
