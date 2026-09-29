# Zaldi-2026

**Akhil Logistics** - A modern Android delivery application for real-time logistics tracking and management.

## Features

- 🚚 Real-time driver location tracking
- 📍 GPS-based route optimization
- 🔔 Push notifications
- 🌐 Google Sign-In integration
- 📱 Adaptive Material Design icons
- 🎨 Material You dynamic theming support

## Project Structure

```
├── res/
│   ├── drawable/          # App icons and vector drawables
│   │   ├── ic_launcher_*.xml       # Adaptive launcher icons
│   │   ├── ic_google.xml          # Google sign-in icon
│   │   └── ic_empty_box.xml       # Empty state illustration
│   └── values/
│       ├── colors.xml      # Color palette
│       ├── strings.xml     # App strings
│       └── themes.xml      # Theme definitions
├── AndroidManifest.xml     # App configuration
└── README.md              # This file
```

## Permissions

The app requires the following permissions:

- `INTERNET` - For API communication
- `ACCESS_FINE_LOCATION` - For precise GPS tracking
- `ACCESS_COARSE_LOCATION` - For approximate location
- `FOREGROUND_SERVICE_LOCATION` - For background location updates
- `POST_NOTIFICATIONS` - For push notifications

## Services

### DriverLocationService

A foreground service that continuously tracks driver location in real-time.

## Configuration

Set your Google Maps API key in the `AndroidManifest.xml`:

```xml
<meta-data
    android:name="com.google.android.geo.API_KEY"
    android:value="YOUR_API_KEY_HERE" />
```

## Building

```bash
./gradlew build
```

## Installation

```bash
./gradlew installDebug
```

## License

None specified.
