<h1>Weather App</h1>

<p>This <strong>Weather App</strong> is built using Flutter and GetX for state management. It provides users with real-time weather data based on their current location, including current conditions, hourly forecasts, daily forecasts, and additional weather-related metrics.</p>

<h2>Features</h2>

<ul>
  <li><strong>Real-Time Weather Data</strong>: Fetches and displays up-to-date weather information by interacting with a weather API.</li>
  <li><strong>Location-Based Weather</strong>: Automatically retrieves the user's location and provides weather data for that specific location.</li>
  <li><strong>GetX State Management</strong>: Efficiently manages the app state and dependencies using GetX, ensuring a smooth and responsive user experience.</li>
  <li><strong>Data Fetching</strong>:
    <ul>
      <li><strong>API Integration</strong>: The app retrieves weather data using an API call, processing the data to display current, hourly, and daily weather information.</li>
      <li><strong>Weather Data Models</strong>: Utilizes data models to parse and manage different types of weather data:
        <ul>
          <li><strong>Current Weather</strong>: Contains current weather conditions.</li>
          <li><strong>Hourly Weather</strong>: Provides hourly weather forecasts.</li>
          <li><strong>Daily Weather</strong>: Shows daily weather forecasts.</li>
        </ul>
      </li>
    </ul>
  </li>
  <li><strong>Custom UI Components</strong>:
    <ul>
      <li><strong>Current Weather Widget</strong>: Displays the current temperature and weather conditions.</li>
      <li><strong>Hourly Data Widget</strong>: Provides an hourly forecast.</li>
      <li><strong>Daily Data Forecast</strong>: Shows a forecast for the coming days.</li>
      <li><strong>Comfort Level Widget</strong>: Displays comfort-related metrics such as humidity and wind speed.</li>
    </ul>
  </li>
  <li><strong>Loading Indicator</strong>: Shows a loading screen with an animated icon and progress indicator while fetching data.</li>
</ul>

<h2>Getting Started</h2>

<p>To run this app locally:</p>

<ol>
  <li><strong>Clone the repository</strong>:
    <pre><code>git clone https://github.com/Kamran-ali39/The-Weather-App.git</code></pre>
  </li>
  <li><strong>Navigate to the project directory</strong>:
    <pre><code>cd The-Weather-App</code></pre>
  </li>
  <li><strong>Install dependencies</strong>:
    <pre><code>flutter pub get</code></pre>
  </li>
  <li><strong>Run the app</strong>:
    <pre><code>flutter run</code></pre>
  </li>
</ol>

<h2>Project Structure</h2>

<ul>
  <li><strong><code>main.dart</code></strong>: The entry point of the application, setting up the main app widget using GetMaterialApp and navigating to the HomeScreen.</li>
  <li><strong><code>home_screen.dart</code></strong>: The main screen where all weather-related data is displayed. It integrates various widgets to present current, hourly, and daily weather data.</li>
  <li><strong><code>global_controller.dart</code></strong>: Manages the state of the weather data and handles data fetching based on the user's current location using Geolocator and GetX.
    <ul>
      <li><strong>Location Handling</strong>: Uses the Geolocator package to request and obtain the user's location.</li>
      <li><strong>Weather Data Management</strong>: Fetches weather data based on the user's location and updates the app state.</li>
      <li><strong>Loading State Management</strong>: Manages the loading state of the app, displaying a loading screen until data is available.</li>
    </ul>
  </li>
  <li><strong><code>fetch_weather_api.dart</code></strong>: Handles API requests to retrieve weather data based on latitude and longitude. Processes the JSON response to create instances of weather data models.</li>
  <li><strong><code>weather_data.dart</code></strong>: Aggregates different types of weather data (current, hourly, daily) into a single <code>WeatherData</code> class for easy access.
    <ul>
      <li><strong><code>WeatherData</code> Class</strong>: Contains:
        <ul>
          <li><strong><code>current</code></strong>: Current weather conditions.</li>
          <li><strong><code>hourly</code></strong>: Hourly weather forecast.</li>
          <li><strong><code>daily</code></strong>: Daily weather forecast.</li>
        </ul>
      </li>
    </ul>
  </li>
  <li>Widgets:
    <ul>
      <li><strong><code>current_weather_widget.dart</code></strong>: Displays the current weather information.</li>
      <li><strong><code>hourly_data_widget.dart</code></strong>: Shows the hourly weather forecast.</li>
      <li><strong><code>daily_data_forecast.dart</code></strong>: Displays the daily weather forecast.</li>
      <li><strong><code>comfort_level.dart</code></strong>: Provides comfort-related metrics.</li>
      <li><strong><code>header_widget.dart</code></strong>: Contains the header UI component.</li>
    </ul>
  </li>
</ul>

<h2>Customization</h2>

<p><strong>Custom Colors</strong>: The app uses a custom color palette defined in <code>custom_colors.dart</code> for a consistent and visually appealing design.</p>

<h2>Dependencies</h2>

<p>This project uses the following Flutter dependencies:</p>

<ul>
  <li><strong><code>flutter/material.dart</code></strong>: Provides Material Design components and theming support.</li>
  <li><strong><code>get.dart</code></strong>: A powerful Flutter package for state management, dependency injection, and route management.</li>
  <li><strong><code>http.dart</code></strong>: Used to make HTTP requests to fetch weather data from the API.</li>
  <li><strong><code>geolocator.dart</code></strong>: Used to determine the device’s geographic location.</li>
</ul>

<h2>License</h2>

<p>This project is licensed under the MIT License - see the <a href="LICENSE">LICENSE</a> file for details.</p>
