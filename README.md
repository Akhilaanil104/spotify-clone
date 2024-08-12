# 🎵 Spotify Clone

This repository contains a Spotify clone built using Flutter. The app is designed to provide a rich music streaming experience, leveraging the power of Bloc for state management, Firebase for backend services, and a clean architecture to ensure maintainable and scalable code.

## 📚 Packages Used

<ul>
  <li><a href="https://pub.dev/packages/flutter_svg"><strong>flutter_svg</strong></a>: For rendering SVG files, providing scalable and high-quality vector images for the UI.</li>
  <li><a href="https://pub.dev/packages/flutter_bloc"><strong>flutter_bloc</strong></a>: Implements the Bloc pattern to manage state across the app efficiently, promoting a clear separation of concerns.</li>
  <li><a href="https://pub.dev/packages/hydrated_bloc"><strong>hydrated_bloc</strong></a>: Extends <code>flutter_bloc</code> with persistent state, ensuring that the app maintains its state across sessions.</li>
  <li><a href="https://pub.dev/packages/path_provider"><strong>path_provider</strong></a>: Provides access to the file system paths for storing data such as user preferences and cached files.</li>
  <li><a href="https://pub.dev/packages/firebase_core"><strong>firebase_core</strong></a>: Essential Firebase services setup, connecting the app to Firebase's powerful backend services.</li>
  <li><a href="https://pub.dev/packages/firebase_auth"><strong>firebase_auth</strong></a>: Handles user authentication, allowing users to sign up, log in, and manage their accounts securely.</li>
  <li><a href="https://pub.dev/packages/cloud_firestore"><strong>cloud_firestore</strong></a>: Provides real-time database services, used for storing user data, playlists, and more.</li>
  <li><a href="https://pub.dev/packages/get_it"><strong>get_it</strong></a>: A simple service locator for dependency injection, making it easier to manage and inject dependencies across the app.</li>
  <li><a href="https://pub.dev/packages/dartz"><strong>dartz</strong></a>: Functional programming utilities, including <code>Either</code>, <code>Option</code>, and more, to handle errors and nullable types more effectively.</li>
  <li><a href="https://pub.dev/packages/just_audio"><strong>just_audio</strong></a>: A feature-rich audio player that supports multiple audio formats, streams, and more, providing the core functionality for music playback.</li>
</ul>

## 🏗️ Clean Architecture

<p>The app is built following the principles of Clean Architecture, ensuring that the code is easy to test, maintain, and extend. The project is organized into several layers:</p>

<ul>
  <li><strong>Presentation Layer</strong>: Contains the UI and state management logic. This layer interacts with the underlying layers via Bloc and displays the data to the user.</li>
  <li><strong>Domain Layer</strong>: Contains the business logic of the app, including use cases, repositories, and entities. This layer is independent of the data sources, allowing for easy testing and flexibility.</li>
  <li><strong>Data Layer</strong>: Manages data retrieval and storage, interacting with Firebase and other APIs. This layer includes models, mappers, and data sources.</li>
</ul>

## 🚀 Getting Started

### Prerequisites

Before you begin, ensure you have the following installed:

<ul>
  <li>Flutter SDK</li>
  <li>Dart</li>
  <li>Firebase CLI (for setting up Firebase)</li>
</ul>

### Installation

<ol>
  <li><strong>Clone the repository</strong>:</li>

  <pre><code>git clone https://github.com/yourusername/spotify_clone.git
cd spotify_clone
  </code></pre>

  <li><strong>Install dependencies</strong>:</li>

  <pre><code>flutter pub get
  </code></pre>

  <li><strong>Set up Firebase</strong>:</li>
  <ul>
    <li>Follow the official Firebase documentation to set up a project and configure Firebase for your Flutter app.</li>
    <li>Add your <code>google-services.json</code> (for Android) and <code>GoogleService-Info.plist</code> (for iOS) to the respective directories.</li>
  </ul>

  <li><strong>Run the app</strong>:</li>

  <pre><code>flutter run
  </code></pre>
</ol>

## 📁 Folder Structure

The project is organized into the following folders:

<ul>
  <li><strong>lib/</strong></li>
  <ul>
    <li><strong>core/</strong>: Contains common utilities, constants, and shared resources.</li>
    <li><strong>data/</strong>: Data sources, models, and repository implementations.</li>
    <li><strong>domain/</strong>: Entities, use cases, and abstract repository definitions.</li>
    <li><strong>presentation/</strong>: UI components, Bloc implementations, and screens.</li>
    <li><strong>injection_container.dart</strong>: Dependency injection setup using <code>get_it</code>.</li>
  </ul>
</ul>

## 🛠️ Features

<ul>
  <li>User Authentication (Firebase Auth)</li>
  <li>Browse and Search for Music</li>
  <li>Create and Manage Playlists</li>
  <li>Stream Music with Just Audio</li>
  <li>Persistent State with Hydrated Bloc</li>
  <li>Scalable and Maintainable Codebase with Clean Architecture</li>
</ul>

## 🎨 UI Design

<p>The UI design for this project was created using Figma. You can view and collaborate on the design by visiting the following link:</p>

<a href="#">Figma Design Link</a> _(Replace with your actual Figma link)_

## 🖥️ Screenshots

<p>Below are some screenshots of the app:</p>

<img src="assets/images/screensimg/screen1.png" alt="Screen 1" width="300">
<img src="assets/images/screensimg/screen2.png" alt="Screen 2" width="300">
<img src="assets/images/screensimg/screen3.png" alt="Screen 3" width="300">

## 🤝 Contributing

<p>Contributions are welcome! Please submit a pull request or open an issue if you have any suggestions or find any bugs.</p>

## 📄 License

<p>This project is licensed under the MIT License. See the <a href="LICENSE">LICENSE</a> file for details.</p>
