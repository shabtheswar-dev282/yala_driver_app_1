# Yala 360 – Driver Mobile Application

> A Flutter-based mobile application developed for safari jeep drivers to improve communication, navigation, safety, and real-time operations within the Yala 360 Safari Management System.

---

## 📱 Project Overview

The **Yala 360 Driver Mobile Application** is part of the **Yala 360 Safari Management System**, developed to assist safari jeep drivers during daily operations.

The application enables authorized drivers to securely log in, share their live GPS location, receive management messages, report wildlife or emergency incidents, and view nearby safari information in real time.

The system integrates **Flutter**, **Firebase Realtime Database**, and **Supabase** to provide a secure, responsive, and real-time experience.

---

## ✨ Features

### 🔐 Secure Driver Login
- Driver authentication using Supabase
- Only authorized drivers can access the application
- Retrieves driver's assigned Jeep ID and Block after login

---

### 🚙 Driver Dashboard
Displays important driver information including:

- Driver ID
- Assigned Jeep ID
- Assigned Safari Block
- Quick access to all driver functions

---

### 📍 Live GPS Tracking
- Real-time GPS location sharing
- Live jeep locations displayed on map
- Automatic location updates
- Nearby jeep visualization

---

### 🗺 Interactive Live Map
Built using **flutter_map** and **OpenStreetMap**

Features include:

- Driver's current location
- Nearby jeep locations
- Zoom controls
- Re-center button
- Live location updates

---

### 🚫 Restricted Zone Monitoring
- Displays restricted areas as polygons
- Detects when a driver enters a restricted zone
- Shows warning dialog
- Haptic vibration alert

---

### 🚨 Incident Reporting
Drivers can report incidents including:

- Animal accidents
- Vehicle breakdowns
- Medical emergencies
- Road blockages
- Illegal activities
- Other emergencies

Each report can include:

- Incident type
- Description
- GPS location
- Photo attachment

Images are uploaded to **Supabase Storage**.

---

### 💬 Management Messaging
Drivers receive messages from management including:

- Announcements
- Safety notices
- Route updates
- Emergency alerts

Supports:

- Message subject
- Full message body
- Attached images
- Read/unread status
- Notification badge

---

### 🌐 Multi-language Support

Drivers can switch the application language instantly.

Supported languages:

- 🇬🇧 English
- 🇱🇰 Sinhala
- 🇮🇳 Tamil

Language changes are applied throughout the application without restarting.

---

### 📲 Custom Splash Screen

The application includes:

- Custom splash screen
- Company branding
- Animated loading effect

---

### 🎨 Custom Login UI

Features include:

- Background image
- Custom logo
- Password show/hide
- Language selector
- Responsive design

---

## 🏗 System Architecture

```
Flutter Mobile App
        │
        │
 ┌──────┴──────────────┐
 │                     │
 │                     │
Firebase RTDB      Supabase
 │                     │
 │                     │
Live GPS         Authentication
Tracking         Driver Database
Nearby Jeeps     Messages
Restricted Zones Incidents
                 Image Storage
```

---

## 🛠 Technology Stack

### Mobile Development

- Flutter
- Dart

### Backend

- Supabase

### Database

- Supabase PostgreSQL
- Firebase Realtime Database

### Authentication

- Supabase Authentication

### Cloud Storage

- Supabase Storage

### Maps

- flutter_map
- OpenStreetMap

### Location Services

- Geolocator

### State Management

- Provider

### Image Loading

- Cached Network Image

### Version Control

- Git
- GitHub

### CI/CD

- GitHub Actions

### IDE

- Android Studio
- VS Code

---

## 📂 Project Structure

```
lib/
│
├── core/
│   ├── constants/
│   ├── services/
│   └── translations/
│
├── features/
│   ├── auth/
│   ├── dashboard/
│   ├── map/
│   ├── incidents/
│   ├── messages/
│   └── splash/
│
├── firebase_options.dart
├── main.dart
│
assets/
│
├── images/
├── icon/
```

---

## 🔥 Firebase Usage

Firebase Realtime Database is used for:

- Live driver locations
- Nearby jeep tracking
- Restricted zones
- Real-time updates

---

## 🟢 Supabase Usage

Supabase is used for:

- Driver authentication
- Driver information
- Incident reports
- Management messages
- Image uploads
- File storage

---

## 📸 Screens

The application includes:

- Splash Screen
- Login Screen
- Driver Dashboard
- Live Map
- Incident Report
- Messages
- Multi-language UI

---

## 🚀 CI/CD

GitHub Actions is configured to automatically:

- Install Flutter dependencies
- Build Android release (.AAB)
- Generate release artifacts
- Verify project builds successfully

---

## 📦 Build

Generate APK

```bash
flutter build apk --release
```

Generate Android App Bundle

```bash
flutter build appbundle --release
```

---

## ▶ Running the Project

Clone the repository

```bash
git clone https://github.com/shabtheswar-dev282/yala360-driver-app.git
```

Go into the project

```bash
cd yala360-driver-app
```

Install dependencies

```bash
flutter pub get
```

Run the application

```bash
flutter run
```

---

## 📋 Requirements

- Flutter SDK
- Dart SDK
- Android Studio
- Firebase Project
- Supabase Project

---

## 📚 Learning Outcomes

This project demonstrates practical experience in:

- Flutter Mobile Development
- Firebase Realtime Database
- Supabase Integration
- RESTful Backend Integration
- Authentication
- GPS Tracking
- Maps Integration
- State Management
- Image Upload
- Cloud Storage
- Multilingual Applications
- Git Version Control
- GitHub Actions CI/CD
- Mobile UI/UX Design

---

## 👨‍💻 Author

**Shatheswar**

Undergraduate – Computer Science

**Project:** Yala 360 Safari Management System

**Module:** Software Development Group Project (SDGP)

---

## 📄 License

This project was developed for academic purposes as part of the Computer Science undergraduate curriculum.
