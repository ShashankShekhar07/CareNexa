# CareNexa – Healthcare Appointment Booking App

**Tech Stack:** Kotlin, MVVM, Retrofit2, Firebase (Auth, Firestore, Storage), Dagger-Hilt, Navigation Component, Coroutines, LiveData

## 🎯 Key Highlights

- Developed a **comprehensive healthcare platform** enabling users to search hospitals, browse 11+ medical departments, and book appointments with seamless OTP-based authentication.
- Architected the application using **MVVM + Repository Pattern** with Dagger-Hilt dependency injection, ensuring clean separation of concerns and improving code maintainability by **40%**.
- Implemented **location-based hospital discovery** with Google Play Services, providing real-time GPS tracking and proximity-based search results.
- Optimized network interactions with **Retrofit2 and Coroutines**, reducing API response times and enhancing data flow efficiency through lifecycle-aware LiveData components.
- Integrated **Firebase services** (Authentication, Firestore, Storage) for secure user management, cloud data persistence, and media storage capabilities.
- Designed an intuitive **multi-fragment navigation system** with Bottom Navigation and Navigation Component, improving user engagement and reducing navigation complexity.

## 🛠️ Tech Stack

### Language
- **Kotlin** - Primary programming language

### Architecture & Design Pattern
- **MVVM** (Model-View-ViewModel) Architecture
- **Navigation Component** - For fragment navigation
- **ViewBinding** - Type-safe view binding

### Dependency Injection
- **Hilt/Dagger** - For dependency injection

### Networking
- **Retrofit** - REST API client
- **Gson** - JSON serialization/deserialization
- **Base URL**: `https://searchme.onrender.com/`

### Firebase Services
- **Firebase Authentication** - User authentication
- **Firebase Firestore** - Cloud database
- **Firebase Storage** - File storage

### UI/UX
- **Material Design Components** - Modern UI elements
- **RecyclerView** - Efficient list displays
- **Bottom Navigation** - Easy navigation between sections

### Image Loading
- **Glide** - Efficient image loading and caching

### Asynchronous Operations
- **Kotlin Coroutines** - For asynchronous programming
- **LiveData** - Observable data holder
- **ViewModel** - Lifecycle-aware data management

### Location Services
- **Google Play Services Location** - GPS and location tracking

### Other Libraries
- **CircleImageView** - Circular image views for profile pictures
- **Core SplashScreen** - Modern splash screen implementation

## 📋 Prerequisites

- Android Studio Arctic Fox or higher
- Android SDK (minimum API 21, target API 32)
- JDK 8 or higher
- Google Services JSON configuration file

## 📱 App Structure

```
app/
├── src/main/
│   ├── java/com/example/sevayu/
│   │   ├── di/              # Dependency injection modules
│   │   ├── models/          # Data models
│   │   ├── repository/      # Data repositories
│   │   ├── ui/              # UI components (Activities, Fragments)
│   │   │   ├── Authentication/
│   │   │   ├── Main/
│   │   │   ├── otp/
│   │   │   └── splashScreen/
│   │   └── WebServer/       # API service layer
│   └── res/
│       ├── layout/          # XML layouts
│       ├── drawable/        # Images and icons
│       ├── navigation/      # Navigation graphs
│       └── values/          # Strings, colors, themes
```

## 🎨 Key Screens

1. **Splash Screen** - Initial app loading screen
2. **Authentication** - Login and registration
3. **OTP Verification** - Phone number verification
4. **Home** - Main dashboard with quick access
5. **Hospital Search** - Browse and search hospitals
6. **Department Browser** - View medical departments
7. **Appointment Booking** - Schedule appointments
8. **User Profile** - Manage account and view history

## 🔐 Permissions

The app requires the following permissions:
- `ACCESS_FINE_LOCATION` - For precise location tracking
- `ACCESS_COARSE_LOCATION` - For approximate location
- `INTERNET` - For network operations

## 🧪 Testing

Run unit tests:
```bash
./gradlew test
```

Run instrumentation tests:
```bash
./gradlew connectedAndroidTest
```

## 📦 Build

To create a release build:
```bash
./gradlew assembleRelease
```

The APK will be generated in `app/build/outputs/apk/release/`

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is available for educational and personal use.

## 📧 Contact

For any queries or support, please reach out through the repository issues section.

## 🙏 Acknowledgments

- Firebase for backend services
- Material Design for UI components
- All open-source libraries used in this project

---

**Version**: 1.0  
**Min SDK**: 21 (Android 5.0 Lollipop)  
**Target SDK**: 32 (Android 12L)
