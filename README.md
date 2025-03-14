# Weather App Compose

A modern Android weather application built with Jetpack Compose that fetches real-time weather data using the WeatherAPI.com service.

## 🌟 Features

- Real-time weather data fetching
- City-based weather search
- Temperature display in Celsius
- Material Design UI with Jetpack Compose
- Clean and minimal interface

## 🛠️ Tech Stack

- **Language**: Kotlin
- **UI Framework**: Jetpack Compose
- **Networking**: Volley
- **API**: WeatherAPI.com
- **Min SDK**: Android 7.0 (API 24)
- **Target SDK**: Android 12 (API 31)

## 📱 Screenshots

[Add screenshots here]

## ⚙️ Setup

### Prerequisites

- Android Studio Arctic Fox or newer
- JDK 11
- Android SDK
- WeatherAPI.com API key

### API Configuration

The app uses WeatherAPI.com for weather data. You'll need to:

1. Sign up at [WeatherAPI.com](https://www.weatherapi.com)
2. Get your API key
3. Replace the API key in `MainActivity.kt`:

```kotlin
const val API_KEY = "your_api_key_here"
```

## 📦 Dependencies

```gradle
dependencies {
    implementation 'androidx.core:core-ktx:1.7.0'
    implementation 'com.android.volley:volley:1.2.1'
    implementation "androidx.compose.ui:ui:$compose_version"
    implementation "androidx.compose.material:material:$compose_version"
    implementation "androidx.compose.ui:ui-tooling-preview:$compose_version"
    implementation 'androidx.lifecycle:lifecycle-runtime-ktx:2.3.1'
    implementation 'androidx.activity:activity-compose:1.3.1'
}
```

## 🏗️ Project Structure

```
app/
├── src/
│   ├── main/
│   │   ├── java/com/trasty/weatherappcompose/
│   │   │   ├── MainActivity.kt
│   │   │   └── ui/theme/
│   │   ├── res/
│   │   │   └── ...
│   │   └── AndroidManifest.xml
│   ├── test/
│   └── androidTest/
```

## 🚀 Installation

1. Clone the repository:

```bash
git clone [repository-url]
```

2. Open in Android Studio:

   - File → Open → Select project directory

3. Build the project:

   - Build → Make Project

4. Run on emulator or device:
   - Run → Run 'app'

## 🔑 API Usage

The app uses WeatherAPI.com with the following endpoint:

```kotlin
https://api.weatherapi.com/v1/current.json?key=$API_KEY&q=$city&aqi=no
```

Response format:

```json
{
    "current": {
        "temp_c": "20.0",
        ...
    }
}
```

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

[Add License Information]

## 📞 Contact

[Add Contact Information]

## 🙏 Acknowledgments

- [WeatherAPI.com](https://www.weatherapi.com) for weather data
- Jetpack Compose documentation
- Material Design guidelines
