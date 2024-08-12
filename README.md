# 🎵 Spotify Clone

This repository contains a Spotify clone built using Flutter. The app is designed to provide a rich music streaming experience, leveraging the power of Bloc for state management, Firebase for backend services, and a clean architecture to ensure maintainable and scalable code.

## 📚 Packages Used

- [**flutter_svg**](https://pub.dev/packages/flutter_svg): For rendering SVG files, providing scalable and high-quality vector images for the UI.
- [**flutter_bloc**](https://pub.dev/packages/flutter_bloc): Implements the Bloc pattern to manage state across the app efficiently, promoting a clear separation of concerns.
- [**hydrated_bloc**](https://pub.dev/packages/hydrated_bloc): Extends `flutter_bloc` with persistent state, ensuring that the app maintains its state across sessions.
- [**path_provider**](https://pub.dev/packages/path_provider): Provides access to the file system paths for storing data such as user preferences and cached files.
- [**firebase_core**](https://pub.dev/packages/firebase_core): Essential Firebase services setup, connecting the app to Firebase's powerful backend services.
- [**firebase_auth**](https://pub.dev/packages/firebase_auth): Handles user authentication, allowing users to sign up, log in, and manage their accounts securely.
- [**cloud_firestore**](https://pub.dev/packages/cloud_firestore): Provides real-time database services, used for storing user data, playlists, and more.
- [**get_it**](https://pub.dev/packages/get_it): A simple service locator for dependency injection, making it easier to manage and inject dependencies across the app.
- [**dartz**](https://pub.dev/packages/dartz): Functional programming utilities, including `Either`, `Option`, and more, to handle errors and nullable types more effectively.
- [**just_audio**](https://pub.dev/packages/just_audio): A feature-rich audio player that supports multiple audio formats, streams, and more, providing the core functionality for music playback.

## 🏗️ Clean Architecture

The app is built following the principles of Clean Architecture, ensuring that the code is easy to test, maintain, and extend. The project is organized into several layers:

- **Presentation Layer**: Contains the UI and state management logic. This layer interacts with the underlying layers via Bloc and displays the data to the user.
- **Domain Layer**: Contains the business logic of the app, including use cases, repositories, and entities. This layer is independent of the data sources, allowing for easy testing and flexibility.
- **Data Layer**: Manages data retrieval and storage, interacting with Firebase and other APIs. This layer includes models, mappers, and data sources.

## 🚀 Getting Started

### Prerequisites

Before you begin, ensure you have the following installed:

- Flutter SDK
- Dart
- Firebase CLI (for setting up Firebase)

### Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/spotify_clone.git
   cd spotify_clone

