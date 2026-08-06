# Experiment 3: Fragments and Debugging in Android

## Objective
Develop an Android application using Fragments to create a flexible user interface. The application displays a list of items in one Fragment and the details of the selected item in another Fragment. The project also demonstrates the use of Android Studio debugging tools, including Breakpoints and Conditional Breakpoints.

---

## Features
- Displays a list of programming-related items.
- Shows details of the selected item in a separate Fragment.
- Uses Fragment Transactions for navigation.
- Supports different screen sizes using Fragments.
- Demonstrates Android Studio Debug Mode.
- Implements both Normal Breakpoint and Conditional Breakpoint.

---

## Technologies Used
- Android Studio
- Kotlin
- Android SDK
- Fragments
- ListView
- ConstraintLayout
- Gradle

---

## Project Structure

```
FragmentDemo
│
├── MainActivity.kt
├── ListFragment.kt
├── DetailFragment.kt
│
├── res
│   ├── layout
│   │   ├── activity_main.xml
│   │   ├── fragment_list.xml
│   │   └── fragment_detail.xml
│   └── values
│
└── AndroidManifest.xml
```

---

## Working

1. The application starts with two Fragments.
2. The left Fragment displays a list of items:
   - Android
   - Java
   - Kotlin
   - Python
   - Spring Boot
3. When the user selects an item, the Detail Fragment updates and displays the selected item.
4. Fragment Transactions are used to replace the Detail Fragment dynamically.

---

## Debugging

### Normal Breakpoint
- Placed inside `DetailFragment`.
- Stops execution every time the Fragment is created.
- Used to inspect variables, lifecycle, and call stack.

### Conditional Breakpoint
- Placed inside `ListFragment`.
- Condition:
```kotlin
selectedItem == "Android"
```
- Stops execution only when **Android** is selected.

---

## Learning Outcomes
- Understanding Android Fragments.
- Fragment Lifecycle.
- Fragment Transactions.
- Communication between Activity and Fragments.
- Debugging using Android Studio.
- Difference between Normal and Conditional Breakpoints.

---

## Output

### List Fragment
Displays a list of available technologies.

### Detail Fragment
Displays the selected technology.

---

## Author

**Komal Kumari**

BCA Graduate (2025)

---

## Repository

Mobile App Development Lab - Experiment 3
