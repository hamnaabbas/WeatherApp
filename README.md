# WeatherApp
Weather Dashboard with Chatbot Integration
Project Overview
This project is a fully responsive Weather Dashboard that utilizes the OpenWeather API for real-time weather data, the Dialogflow API for chatbot functionality, and Chart.js for data visualization. The dashboard provides users with current weather information, a 5-day forecast, and various visualizations to enhance the understanding of weather trends.

Features
User Input: An input box allows users to enter a city name and retrieve weather data.
Current Weather Widget: Displays essential weather details such as temperature, humidity, wind speed, and weather description. The background changes according to the weather condition.
5-Day Weather Forecast: Displays daily forecasts, including temperatures and weather conditions.
Data Visualizations:
Vertical Bar Chart for 5-day temperatures.
Doughnut Chart showing the distribution of weather conditions over the 5-day period.
Line Chart illustrating temperature changes over the forecast period.
Chatbot Integration: A chatbot responds to user inquiries about the weather data, providing insights like highest, lowest, and average temperatures.
Pagination for Forecast Table: Displays the first 10 entries of the temperature forecast with pagination for easier navigation.
Technologies Used
1.Frontend: HTML, CSS, JavaScript (vanilla or jQuery)
2.APIs: OpenWeather API, Dialogflow API
3.Data Visualization: Chart.js
4.Setup Instructions
5.Step 1: OpenWeather API Setup
6.Create an API Key:
Sign up at OpenWeather.
7.Confirm your email address.
8.Generate an API key from your dashboard.
9.API Documentation Overview:
Current Weather Data:
Request format:
bash
Copy code:
                     https://api.openweathermap.org/data/2.5/weather?q={city name}&appid={API key}&units=metric
5-Day Forecast Data:
Request format:
bash
Copy code:
                     https://api.openweathermap.org/data/2.5/forecast?q={city name}&appid={API key}
Step 2: Frontend Layout
HTML Structure:

Create a simple layout with:
An input box for city names.
A "Get Weather" button.
Sections for current weather and 5-day forecast.
CSS Styling:

Style the dashboard for responsiveness using Flexbox or Grid.
Add a weather-themed background image or gradient.
Step 3: Integrating the API
Fetching Current Weather Data:

Use Fetch API or AJAX to get weather data when the user submits a city name.
Extract and display the following:
City name, temperature (allow switching between Celsius and Fahrenheit), humidity, wind speed, and weather description.
Fetching 5-Day Weather Forecast:

Make an API call to the forecast endpoint to retrieve and display a 5-day weather forecast.
Error Handling:

Implement error handling for scenarios like invalid city names or API failures.
Display friendly messages such as "City not found" or "API limit reached".
Optimizing API Calls:

Prevent unnecessary API calls by checking if the input city name has changed before making a request.
Data Visualization
Chart.js Integration
Use Chart.js to create three types of charts:
Vertical Bar Chart: Shows the temperature for the next 5 days, with animation delays.
Doughnut Chart: Displays the distribution of weather conditions, with animation delays.
Line Chart: Illustrates temperature changes over the forecast period, with drop animations.
Using the Dashboard
Open the dashboard in your web browser.
Enter a city name in the input box and click "Get Weather."
View the current weather information and 5-day forecast.
Explore the charts for visual representation of the data.
Interact with the chatbot to ask questions related to the displayed weather data.
