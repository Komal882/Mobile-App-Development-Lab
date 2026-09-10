#  CampusConnect – Student Service

## Mobile Application Development – Test 01

**CampusConnect** is a scenario-based Android application developed to provide students with basic campus services. The application demonstrates the use of **Activities, Fragments, Intents, Android UI components, Activity Lifecycle methods, and Notifications**.

---

##  Aim

To develop and demonstrate an Android application named **CampusConnect** that allows students to view their profile and register for a course using Android **Activities, Fragments, Intents, UI components, Activity Lifecycle methods, and Notifications**.

---

##  Technologies Used

- **Android Studio**
- **Kotlin**
- **XML**
- **Android SDK**
- **Gradle**
- **Android Logcat**

---

##  Application Features

###  1. Home Activity

The Home screen contains:

- College/application logo
- Application name – **CampusConnect**
- Welcome message
- **Student Profile** button
- **Course Registration** button

###  2. Student Profile Fragment

The Profile Fragment displays:

- Student Name
- USN
- Email
- Gender using **RadioButton** and **RadioGroup**

###  3. Course Registration Fragment

The Course Registration Fragment contains:

- Course Name using **EditText**
- Semester selection using **RadioButton** and **RadioGroup**
- **Register** button

###  4. Registration Confirmation Activity

After clicking Register:

- An **Intent** sends the selected course and semester.
- A confirmation screen displays the registration result.
- A **Back to Home** button is provided.

###  5. Android Notification

After successful registration, the application displays an Android notification:

> **Course Registration**  
> Course registered successfully

###  6. Activity Lifecycle

Lifecycle methods are demonstrated and logged in Logcat:

```text
onCreate()
    ↓
onStart()
    ↓
onResume()
    ↓
onPause()
    ↓
onStop()
    ↓
onDestroy()
```

---

##  Project Flow

```text
                  ┌────────────────────┐
                  │    HOME ACTIVITY   │
                  └─────────┬──────────┘
                            │
              ┌─────────────┴─────────────┐
              ↓                           ↓
    ┌──────────────────┐       ┌────────────────────────┐
    │ Profile Fragment │       │ Course Registration    │
    │                  │       │ Fragment               │
    └──────────────────┘       └───────────┬────────────┘
                                           │
                                  Enter Course Name
                                           +
                                  Select Semester
                                           │
                                           ↓
                                      REGISTER
                                           │
                                           ↓
                              ┌────────────────────────┐
                              │ Confirmation Activity  │
                              └───────────┬────────────┘
                                          │
                              ┌───────────┴───────────┐
                              ↓                       ↓
                    Registration Result       Android Notification
                              │
                              ↓
                       Back to Home
```

---

##  Project Structure

```text
CampusConnect/
│
├── app/
│   └── src/main/
│       ├── java/com/example/campusconnect/
│       │   ├── MainActivity.kt
│       │   ├── ProfileFragment.kt
│       │   ├── CourseRegistrationFragment.kt
│       │   └── ConfirmationActivity.kt
│       │
│       ├── res/
│       │   └── layout/
│       │       ├── activity_main.xml
│       │       ├── fragment_profile.xml
│       │       ├── fragment_course_registration.xml
│       │       └── activity_confirmation.xml
│       │
│       └── AndroidManifest.xml
│
└── README.md
```

---

#  Application Screenshots

The screenshots are stored inside the `screenshots` folder so that GitHub displays them directly in this README.

## 1.  Home Screen

![CampusConnect Home Screen](./screenshots/home.png)

---

## 2.  Course Registration

![Course Registration](./screenshots/course-registration.png)

---

## 3.  Registration Confirmation

![Registration Confirmation](./screenshots/confirmation.png)

---

## 4.  Registration Notification

![Registration Notification](./screenshots/notification.png)

---

##  Test Case

### Input

```text
Course Name : MCA
Semester    : Semester 1
```

### Expected Output

```text
Registration Successful

Course: MCA
Semester: Semester 1
```

The application also generates a notification confirming successful course registration.

---

##  How to Run

1. Open the project in **Android Studio**.
2. Wait for Gradle synchronization to complete.
3. Connect an Android device or start an Emulator.
4. Select the device.
5. Click **Run ▶**.
6. Open **Student Profile** to view profile information.
7. Open **Course Registration**.
8. Enter the course name.
9. Select a semester.
10. Click **Register**.
11. Verify the confirmation screen and notification.
12. Check lifecycle events in **Logcat**.

---

##  Result

The **CampusConnect – Student Service** Android application was successfully developed and tested. The project demonstrates **Activities, Fragments, Intents, UI Views, RadioButtons, RadioGroup, EditText, Buttons, Notifications, and Activity Lifecycle methods**.

---

##  Conclusion

The project provides practical understanding of Android application development by integrating multiple Android components into one scenario-based application. It successfully implements student profile viewing, course registration, Intent-based navigation, registration confirmation, lifecycle logging, and notification generation.

---

##  Project Information

| Item | Details |
|---|---|
| Project | CampusConnect – Student Service |
| Test | Test 01 |
| Platform | Android |
| Language | Kotlin |
| UI | XML |
| IDE | Android Studio |
| Application Type | Student Service App |
