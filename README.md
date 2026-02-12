# Mars Photos

> Learning REST APIs and network operations in Android

An Android app that fetches and displays real photos from Mars taken by NASA's rovers. Built as part of **Android Basics with Compose - Unit 5, Pathway 1** to learn how to connect to the internet and retrieve data from web services.

---

## 🚀 About

**Mars Photos** is a learning project that demonstrates how to make network requests in Android apps. The app connects to NASA's Mars Rover Photos API and displays images in a grid layout using Jetpack Compose.

This project is part of Google's **Android Basics with Compose** course:
- **Unit 5**: Connect to the internet
- **Pathway 1**: Get data from the internet

---

## 🎯 Learning Objectives

This project helped me understand:

- **REST APIs**: Making HTTP requests to web services
- **Retrofit**: Setting up and using the Retrofit library
- **JSON Parsing**: Deserializing JSON data with kotlinx.serialization
- **Coroutines**: Handling asynchronous operations
- **Repository Pattern**: Separating data sources from UI logic
- **Error Handling**: Managing network errors and loading states
- **Coil**: Loading and displaying images from URLs

---

## ✨ Features

- **Fetch Mars Photos**: Retrieves real images from NASA's API
- **Grid Display**: Shows photos in a responsive grid layout
- **Loading States**: Displays loading indicator while fetching data
- **Error Handling**: Shows error messages when network requests fail
- **Offline Support**: Graceful handling of network unavailability

---

## 🛠️ Tech Stack

- **Language**: Kotlin
- **UI Framework**: Jetpack Compose
- **Architecture**: MVVM with Repository pattern
- **Networking**: Retrofit
- **JSON Serialization**: kotlinx.serialization
- **Image Loading**: Coil
- **Async Operations**: Kotlin Coroutines
- **Build System**: Gradle (Kotlin DSL)

---

## 📡 API Used

**NASA Mars Rover Photos API**
- Provider: NASA Open APIs
- Endpoint: Mars Rover Photos
- Data: Real photos taken by Mars rovers

---

## 🚀 Getting Started

### Prerequisites

- Android Studio (latest stable version)
- JDK 8 or higher
- Internet connection (for API requests)

### Installation

1. **Clone the repository**:
```bash
   git clone https://github.com/SamratVsn/Mars-Photos.git
```

2. **Open in Android Studio**:
   - Launch Android Studio
   - Select "Open an Existing Project"
   - Navigate to the cloned directory

3. **Run the app**:
   - Connect an Android device or start an emulator
   - Ensure the device/emulator has internet access
   - Click the "Run" button (▶️)

---

## 📚 Key Concepts Learned

### REST API Integration
- Understanding RESTful web services
- Making GET requests with Retrofit
- Parsing JSON responses

### Asynchronous Programming
- Using Kotlin Coroutines for network calls
- Managing background threads
- Updating UI from coroutines

### Repository Pattern
- Separating data layer from UI
- Creating a single source of truth
- Making code more testable

### State Management
- Handling loading, success, and error states
- Updating UI based on network response
- Managing app state with ViewModel

---

## 🧩 App Architecture
```
app/
├── data/
│   └── MarsPhotosRepository.kt     # Data source
├── model/
│   └── MarsPhoto.kt                # Data model
├── network/
│   └── MarsApiService.kt           # Retrofit service
├── ui/
│   ├── screens/
│   │   └── MarsPhotosScreen.kt     # Main UI
│   └── MarsViewModel.kt            # ViewModel
└── MarsPhotosApplication.kt        # Application class
```

---

## 🔄 How It Works

1. **App launches** → ViewModel initiates API call
2. **Retrofit makes request** → Fetches data from NASA API
3. **JSON response** → Parsed into Kotlin data classes
4. **Images displayed** → Coil loads images into LazyVerticalGrid
5. **Error handling** → Shows appropriate message if request fails

---

## 💡 What I Learned

- How to integrate REST APIs in Android apps
- Setting up Retrofit with kotlinx.serialization
- Managing network operations with coroutines
- Handling different UI states (loading, success, error)
- Loading remote images efficiently with Coil
- Implementing the repository pattern for clean architecture

---

## 🤝 Acknowledgments

Built following Google's **Android Basics with Compose** course:
- [Unit 5 - Pathway 1: Get data from the internet](https://developer.android.com/courses/pathways/android-basics-compose-unit-5-pathway-1)

---

## 📄 License

This project is open source and available for educational purposes.

---

> "Connecting to the internet, one API call at a time."
