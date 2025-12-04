Weather App



 multi-page Flutter application that retrieves real-time weather data using the OpenWeatherMap API..

Features

Core Requirements Implemented

Multi-Page Navigation: Home/Search, Details, Favorites, and Settings screens.

Real-Time Data: Fetches current temperature, humidity, wind speed, sunrise/sunset, and "feels like" temp.

Search Functionality: Search for any city worldwide with error handling

Favorites System: Save and remove favorite cities using local storage

Settings: Toggle between Metric (°C) and Imperial (°F) units.

State Management: Uses Provider for efficient state handling across screens.

 Creative & Bonus Features

Dynamic "Mood" Backgrounds: The background gradient changes automatically based on the weather condition:

Glassmorphism UI: Custom-built frosted glass widgets for weather details.

Secure API Handling: API keys are separated into a config file (git-ignored) for security.

 Project Structure

The project follows a clean, scalable architecture separating logic from UI:

lib/
├── models/
│   └── weather_model.dart       # JSON parsing logic
├── providers/
│   └── weather_provider.dart    # State Management (Search, Favorites, Settings)
├── screens/
│   ├── home_screen.dart         # Search & Favorites List
│   ├── details_screen.dart      # Detailed weather view with dynamic backgrounds
│   └── settings_screen.dart     # Unit toggle
├── services/
│   └── api_service.dart         # HTTP calls to OpenWeatherMap
├── widgets/
│   └── glass_card.dart          # Reusable frosted glass UI component
├── config.dart                  # (Ignored by Git) Stores API Key
└── main.dart                    # Entry point & Theme setup
