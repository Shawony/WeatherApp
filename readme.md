# Weather App - Text Content Only

## Introduction

This weather app allows users to check the current weather conditions by entering a city or country name. The data is fetched from the OpenWeather API.

## Components

### Search Section

- Input Field: Users enter the city or country name here.
- Search Button: Triggers the weather data retrieval function.

### Weather Display Section

- **Temperature Display**: Shows the current temperature in Celsius.
- **City Display**: Displays the city name corresponding to the weather data.
- **Weather Details**:
  - **Humidity Display**: Displays the current humidity percentage.
  - **Wind Speed Display**: Displays the current wind speed in km/h.

## Functionality

### Weather Checking Logic

- The function `checkWeather(city)` is called when the search button is clicked.
- The app fetches weather data from the OpenWeather API using the URL structure:

https://api.openweathermap.org/data/2.5/weather?&units=metric&q={city}&appid={apiKey}

### Conditions for Displaying Data

- If the input is empty, the app alerts the user to enter a city or country name.
- If the entered city or country is invalid, an error alert is displayed.
- If the request succeeds, the following data points are updated:
  - **City Name**
  - **Temperature**
  - **Humidity**
  - **Wind Speed**

### Icon Mapping (Text-Based Version)

Since this markdown file is text-only, the following weather conditions are represented as text instead of icons:

- **Cloudy** - Display text: "Cloudy Weather"
- **Clear** - Display text: "Clear Sky"
- **Rain** - Display text: "Rainy Weather"
- **Drizzle** - Display text: "Light Rain/Drizzle"
- **Mist** - Display text: "Misty Conditions"
- **Snow** - Display text: "Snowy Weather"

## Example Flow

1. User enters "New York" in the search field.
2. The app fetches data from OpenWeather API.
3. Displayed Data:
   - **City:** New York
   - **Temperature:** 22°C
   - **Humidity:** 50%
   - **Wind Speed:** 15 km/h
   - **Weather Condition:** Rainy Weather

## Error Handling

- **Empty Input:** Alerts the user to enter a valid city or country name.
- **Invalid Location:** Displays an error message indicating invalid input.

This markdown version simplifies the app's interface by removing visual elements like icons while maintaining its core functionality.
