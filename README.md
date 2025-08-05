# 🌤️ Weather App

A beautiful and intuitive Android weather application that provides real-time weather information for any city worldwide. Built with Java and powered by the OpenWeatherMap API.

## 📱 Screenshot
<img width="853" height="428" alt="image" src="https://github.com/user-attachments/assets/5e953da8-b7db-42ac-99e6-afc629ce1d43" />


## ✨ Features

- **Real-time Weather Data**: Get current weather conditions for any city
- **Beautiful UI**: Modern gradient background with clean, user-friendly interface
- **Detailed Information**: 
  - Current temperature
  - Weather description
  - Humidity percentage
  - Wind speed
- **Dynamic Weather Icons**: Weather-appropriate icons that change based on conditions
- **City Search**: Easy city name input with error handling
- **Responsive Design**: Optimized for different screen sizes

## 🛠️ Technologies Used

- **Language**: Java
- **Platform**: Android (API 21+)
- **Networking**: OkHttp3 for API calls
- **API**: OpenWeatherMap API
- **UI**: RelativeLayout with custom backgrounds
- **Fonts**: Urbanist font family

## 📋 Prerequisites

- Android Studio Arctic Fox or later
- Android SDK (API level 21 or higher)
- Internet connection for weather data

## 🚀 Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/saemanab/WeatherApp.git
   ```

2. **Open in Android Studio**
   - Launch Android Studio
   - Select "Open an Existing Project"
   - Navigate to the cloned repository folder

3. **Get API Key**
   - Visit [OpenWeatherMap](https://openweathermap.org/api)
   - Sign up for a free account
   - Generate your API key

4. **Configure API Key**
   - Open `MainActivity.java`
   - Replace the `API_KEY` constant with your actual API key:
   ```java
   private static final String API_KEY = "your_api_key_here";
   ```

5. **Add Internet Permission**
   - Ensure your `AndroidManifest.xml` includes:
   ```xml
   <uses-permission android:name="android.permission.INTERNET" />
   ```

6. **Build and Run**
   - Connect your Android device or start an emulator
   - Click "Run" in Android Studio

## 📁 Project Structure

```
app/
├── src/main/
│   ├── java/com/example/weatherapp/
│   │   └── MainActivity.java          # Main application logic
│   ├── res/
│   │   ├── drawable/                  # Weather icons and backgrounds
│   │   │   ├── background.xml         # Main gradient background
│   │   │   ├── background2.xml        # Details section background
│   │   │   ├── sun.png               # Default sunny weather icon
│   │   │   ├── humidity.png          # Humidity icon
│   │   │   ├── wind.png              # Wind icon
│   │   │   └── ic_*.png              # OpenWeatherMap weather icons
│   │   ├── font/
│   │   │   └── urbanist.ttf          # Custom font
│   │   ├── layout/
│   │   │   └── activity_main.xml     # Main layout file
│   │   └── values/
│   │       ├── colors.xml            # Color definitions
│   │       └── strings.xml           # String resources
│   └── AndroidManifest.xml           # App configuration
```

## 🎨 Customization

### Adding New Weather Icons
1. Download weather icons (preferably 200x200px)
2. Name them according to OpenWeatherMap icon codes (e.g., `ic_01d.png`, `ic_02n.png`)
3. Place them in the `res/drawable/` folder

### Changing Colors
Edit the colors in `res/values/colors.xml`:
```xml
<color name="white">#FFFFFF</color>
<color name="yellow">#FFBF00</color>
```

### Modifying Background
Update the gradient backgrounds in `res/drawable/background.xml` and `res/drawable/background2.xml`

## 🌐 API Integration

The app uses the OpenWeatherMap Current Weather Data API:
- **Endpoint**: `https://api.openweathermap.org/data/2.5/weather`
- **Parameters**: 
  - `q`: City name
  - `appid`: Your API key
  - `units`: metric (for Celsius)

### API Response Handling
The app processes the following data from the API response:
- City name
- Temperature (°C)
- Weather description
- Humidity (%)
- Wind speed (km/h)
- Weather icon code

## 🔧 Troubleshooting

### Common Issues

1. **No weather data showing**
   - Check your internet connection
   - Verify your API key is correct
   - Ensure `INTERNET` permission is added to AndroidManifest.xml

2. **Icons not displaying**
   - Make sure weather icon files are in the correct format (PNG)
   - Verify icon files are named correctly (`ic_01d.png`, etc.)
   - Check that files are in the `res/drawable/` folder

3. **App crashes on city search**
   - Verify the API URL is correct
   - Check for network connectivity
   - Ensure proper error handling in the code

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👨‍💻 Author
**Your Name**
- Abiaba Mohamed
- Email: mohamedabiaba202@gmail.com

## 🙏 Acknowledgments

- [OpenWeatherMap](https://openweathermap.org/) for providing the weather API
- [OkHttp](https://square.github.io/okhttp/) for networking
- Weather icons from various sources
- Urbanist font family

## 📊 Future Enhancements

- [ ] 7-day weather forecast
- [ ] Location-based weather detection
- [ ] Weather alerts and notifications
- [ ] Multiple city management
- [ ] Weather history and charts
- [ ] Dark/Light theme toggle
- [ ] Weather widgets

---

⭐ If you found this project helpful, please consider giving it a star!


Made with ❤️ for the Android community
