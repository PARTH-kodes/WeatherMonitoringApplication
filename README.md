# Weather Monitoring Application

This is a Spring Boot application for monitoring weather conditions using the OpenWeatherMap API. It allows users to search for weather data by city name and displays current weather conditions, including temperature, pressure, humidity, and wind speed.

## Table of Contents
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Setup Instructions](#setup-instructions)
- [API Key Configuration](#api-key-configuration)
- [Usage](#usage)
- [Code Structure](#code-structure)
- [License](#license)

## Features
- Search for weather data by city name.
- Display current temperature in Celsius or Fahrenheit.
- Show weather description, minimum and maximum temperatures, pressure, humidity, and wind speed.
- Dynamic weather icons based on the current weather conditions.

## Technologies Used
- Spring Boot
- Vaadin for the UI
- OkHttp for making HTTP requests
- JSON for data handling
- Maven for dependency management

## Setup Instructions

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/saadusufzai/WeatherApp.git
   cd WeatherApp
   ```

2. **Install Dependencies**:
   Ensure you have [Maven](https://maven.apache.org/install.html) installed, then run:
   ```bash
   mvn install
   ```

3. **Configure API Key**:
   Open `WeatherService.java` and replace the placeholder API key with your actual OpenWeatherMap API key:
   ```java
   private String APIkey = "YOUR_API_KEY";
   ```

4. **Run the Application**:
   Use Maven to run the Spring Boot application:
   ```bash
   mvn spring-boot:run
   ```

5. **Access the Application**:
   Open a web browser and go to [http://localhost:8080](http://localhost:8080).

## API Key Configuration
To use the OpenWeatherMap API, you must sign up for an API key. Follow these steps:
1. Go to the [OpenWeatherMap website](https://openweathermap.org/).
2. Sign up for an account.
3. Obtain your API key from the account dashboard.
4. Replace the existing `APIkey` in `WeatherService.java` with your new key.

## Usage
- Enter the name of the city in the text field and select the desired temperature unit (Celsius or Fahrenheit).
- Click the search button to fetch and display the weather information for the specified city.

## Code Structure
```plaintext
WeatherApp/
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   ├── com/
│   │   │   │   └── bwap/
│   │   │   │       └── weatherapp/
│   │   │   │           ├── WeatherAppApplication.java
│   │   │   │           ├── controller/
│   │   │   │           │   └── WeatherService.java
│   │   │   │           └── view/
│   │   │   │               └── MainView.java
│   │   └── resources/
│   │       └── application.properties
└── pom.xml
```

## License

This project is open-source and available under the MIT License.