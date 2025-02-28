# my-weather-app

# Weather Forecast App

## Overview

This is a SwiftUI-based Weather Forecast App that provides weather details using an external API. The app features:

- Real-time weather updates
- Forecast for upcoming days
- Beautiful, intuitive UI
- Location support
## API key: http://api.weatherapi.com/v1/forecast.json?key=b94801885e204d72aab141008252702&q=Mumbai&days=7&aqi=no&alerts=no

## Setup Instructions

### Prerequisites

- macOS with Xcode installed (Latest version recommended)
- Swift and SwiftUI knowledge
- An API key from [WeatherAPI](https://www.weatherapi.com/)

### Installation Steps

1. **Clone the Repository:**

   ```sh
   git clone https://github.com/Atharva11c/my-weather-app.git
   cd my-weather-app
   ```

2. **Open Project in Xcode:**

   - Open `my weather app.xcodeproj` in Xcode.

3. **Install Dependencies:**

   - This project uses `Alamofire` for networking. Install dependencies via Swift Package Manager (SPM) if not already added.

4. **Set Up API Key:**

   - Create a file `Config.swift` in the project and add:
     ```swift
     struct Config {
         static let apiKey = "http://api.weatherapi.com/v1/forecast.json?key=b94801885e204d72aab141008252702&q=Mumbai&days=7&aqi=no&alerts=no"
     }
     ```
  

5. **Run the App:**

   - Select an iOS Simulator or connected device.
   - Press `Cmd + R` or click the **Run** button in Xcode.

## Implementation Details

- **Networking:** Uses `Alamofire` to fetch weather data.
- **Data Model:** The `WeatherModel.swift` handles JSON parsing.
- **UI:** `ContentView.swift` and `WeatherDetailView.swift` display weather details with animations and gradients.
- **State Management:** Uses `@State`, `@Binding`, and `@ObservedObject`.

## Design Decisions

- **SwiftUI for modern UI components.**
- **Dark mode support with background color adaptation.**
- **Navigation with **``**.**

## Future Enhancements

- Add hourly forecast view.
- Improve animations and transitions.
- Implement offline caching.

## Contribution

Feel free to fork, improve, and submit a PR!

## License

MIT License. See `LICENSE` for details.

