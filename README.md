# Runes 🗺️ - Local Lore & Story Map

Runes is a native Android application that brings local stories, folklore, and hidden histories to life on an interactive map. It's a community-sourced platform where users can discover the cultural landmarks around them and contribute their own knowledge, creating a shared atlas of stories.

This project is being built by a three-person team to explore modern Android development practices, including a declarative UI with Jetpack Compose, a real-time backend with Firebase, and integration with the Google Maps SDK.

## ✨ Core Features (Planned)

-   **Interactive Story Map:** Browse a map populated with "Runes"—pins representing stories, historical events, or cultural landmarks.
-   **Community Contributions:** Users can submit their own Runes, complete with a title, description, category, and photos.
-   **Google Sign-In:** Secure and easy user authentication using Google accounts.
-   **User Profiles:** A simple profile page to view a user's contributions and activity.
-   **Dynamic Filtering:** Filter the map by categories like "Folklore," "Architecture," or "Historical Events" to customize discovery.
-   **Location-Aware:** The app will use the device's location to highlight nearby Runes and points of interest.

## 📸 Screenshots

*(This section will be updated with screenshots as the UI is developed.)*

| Login Screen | Main Map View | Story Submission |
| :----------: | :-----------: | :--------------: |
| _(Coming Soon)_ | _(Coming Soon)_ | _(Coming Soon)_ |

## 🛠️ Tech Stack & Architecture

-   **UI:** Fully built with [Jetpack Compose](https://developer.android.com/jetpack/compose), Android's modern declarative UI toolkit.
-   **Architecture:** Follows the recommended Android Architecture Components pattern using ViewModel and Repository.
-   **Backend:** [Firebase](https://firebase.google.com/) for a complete backend solution:
    -   **Authentication:** Manages user sign-up and login via Google Sign-In.
    -   **Firestore Database:** A real-time NoSQL database to store all user and Rune data.
    -   **Cloud Storage:** For hosting user-uploaded images.
-   **Mapping:** [Google Maps SDK for Android](https://developers.google.com/maps/android-sdk) and the Maps Compose Library for the interactive map interface.
-   **Asynchronous Operations:** Kotlin Coroutines and Flow for managing background tasks and reactive data streams.

## 🚀 Getting Started

To get a local copy up and running, follow these simple steps.

### Prerequisites

-   Android Studio (latest stable version recommended)
-   An Android device or emulator (API level 24+)
-   A `google-services.json` file from a configured Firebase project.
-   A Google Maps API key.

### Installation

1.  **Clone the repo:**
    ```sh
    git clone [https://github.com/your-username/runes.git](https://github.com/your-username/runes.git)
    ```
2.  **Firebase Setup:**
    -   Download your project's `google-services.json` file from the Firebase Console and place it in the `app/` directory.
3.  **Google Maps API Key:**
    -   Create a `local.properties` file in the root directory of the project.
    -   Add your Google Maps API key to the file like this:
        ```properties
        MAPS_API_KEY="YOUR_API_KEY_HERE"
        ```
4.  Open the project in Android Studio.
5.  Let Gradle sync the dependencies.
6.  Run the app on your emulator or physical device.