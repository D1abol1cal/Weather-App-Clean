# Weather App

A minimal, clean-UI weather app built with Flutter, using the device's location to show current conditions: temperature, humidity, sunrise/sunset, and the day's high/low.

![Flutter](https://img.shields.io/badge/Flutter-02569B?logo=flutter&logoColor=white)
![Dart](https://img.shields.io/badge/Dart-0175C2?logo=dart&logoColor=white)
![BLoC](https://img.shields.io/badge/State-BLoC-6200EE)

## Features

- Automatically detects the device's location (with a permission flow)
- Current temperature, condition, humidity, sunrise and sunset times
- Today's high and low
- State managed with `flutter_bloc`

## Setup

This app uses the [OpenWeatherMap](https://openweathermap.org/api) API. Get a free API key, then run with it passed in at build time — it's never stored in the source:

```bash
flutter pub get
flutter run --dart-define=OPENWEATHER_API_KEY=your_key_here
```

## Tech stack

- `flutter_bloc` + `equatable` for state management
- `geolocator` for device location
- `weather` for the OpenWeatherMap API client
- `intl` for date/time formatting
