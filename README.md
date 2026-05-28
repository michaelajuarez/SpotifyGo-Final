# SpotifyGo

A mobile app that combines Spotify with real-time location to bring music and maps together. Built with React Native for iOS and Android as the final project for CSE 115A (Introduction to Software Engineering) at UC Santa Cruz.

---

## Table of Contents

- [About](#about)
- [Tech Stack](#tech-stack)
- [Features](#features)
- [Project Structure](#project-structure)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
  - [Running the App](#running-the-app)
- [Testing](#testing)
- [Contributors](#contributors)

---

## About

SpotifyGo is a location-aware music app that integrates with the Spotify API. Users log in with their Spotify account and can interact with music content tied to their current location via an interactive map interface. The project was developed by a team of students for CSE 115A at UCSC.

---

## Tech Stack

| Layer | Technology |
|---|---|
| Framework | React Native 0.67 |
| Navigation | React Navigation (Native Stack) |
| Authentication | Spotify OAuth via `react-native-app-auth` |
| Backend / Database | Firebase (Firestore) |
| Maps | React Native Maps |
| Location | `@react-native-community/geolocation`, `react-native-get-location` |
| Icons | React Native Vector Icons |
| Testing | Jest + React Test Renderer |
| Linting | ESLint |

---

## Features

- **Spotify Login** — OAuth 2.0 authentication with a user's Spotify account
- **Interactive Map** — Location-based map view with custom styling
- **Geolocation** — Real-time device location tracking
- **Firebase Integration** — Cloud data storage and retrieval
- **Cross-Platform** — Runs on both iOS and Android

---

## Project Structure

```
SpotifyGo-Final/
├── android/                  # Android native project
├── ios/                      # iOS native project
├── __tests__/                # Jest test files
├── Release_1.0_Documents/    # Project documentation and release notes
├── App.js                    # Root application component
├── index.js                  # App entry point
├── interface.js              # Main UI screens and components
├── interfaceStyle.js         # Stylesheet for UI components
├── mapStyle.js               # Custom map styling
├── babel.config.js
├── metro.config.js
└── package.json
```

---

## Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (v14+)
- [React Native CLI](https://reactnative.dev/docs/environment-setup)
- Xcode (for iOS) or Android Studio (for Android)
- A [Spotify Developer](https://developer.spotify.com/dashboard/) account with a registered app (for OAuth credentials)
- A [Firebase](https://firebase.google.com/) project with Firestore enabled

### Installation

1. Clone the repository:

```bash
git clone https://github.com/michaelajuarez/SpotifyGo-Final.git
cd SpotifyGo-Final
```

2. Install JavaScript dependencies:

```bash
npm install
```

3. Install iOS pods (macOS only):

```bash
cd ios && pod install && cd ..
```

4. Add your Spotify and Firebase credentials to the project (refer to `interface.js` and your Firebase config file).

### Running the App

**iOS:**
```bash
npm run ios
```

**Android:**
```bash
npm run android
```

**Start Metro bundler only:**
```bash
npm start
```

---

## Testing

```bash
npm test
```

Tests are located in the `__tests__/` directory and use Jest with the React Native preset.

---

## Contributors

Built by a team for CSE 115A — Introduction to Software Engineering, UC Santa Cruz.

- Michael Juarez — [@michaelajuarez](https://github.com/michaelajuarez)
