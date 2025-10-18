# Kerala-Weather-prediction-Model
Weather prediction plays a vital role in daily life — from agriculture to transportation and disaster management.
This project, “Kerala Smart Weather Predictor”, uses machine learning to predict the weather of any district in Kerala based on the date selected by the user.
It’s a data-driven system built using Python and Streamlit for real-time prediction and visualization.

The main objectives are:

To develop a machine learning model that can predict future weather conditions for Kerala districts.

To build an interactive web app that allows users to input a district and date.

To demonstrate how data science and AI can help in local-level forecasting and planning.

Why Weather Prediction is Important

Weather prediction is useful for:

Farmers: Helps in deciding irrigation, sowing, and harvesting time.

Construction: Helps in planning outdoor activities safely.

 Transportation: Ensures road, sea, and air transport safety.

 Disaster management: Predicts extreme weather events like floods or heavy rainfall.

 General public: Helps in travel planning and daily preparation.

Tools and Technologies Used
Tool / Library	Purpose
Python	Programming language used
Streamlit	To create the web-based user interface
Pandas	Data manipulation and handling
NumPy	Numerical computation
Scikit-learn	Machine learning model building
RandomForestClassifier	Algorithm used for prediction
LabelEncoder	To convert text data into numerical format

Dataset Description

The dataset used: kerala_district_weather_20000.csv

It contains 20,000+ records across 14 districts of Kerala.

Major columns include:

District

Temperature

Humidity

Pressure

WindSpeed

Precipitation

CloudCover

MonsoonPhase

Weather (Target column)


Methodology / Workflow

Step 1: Data Loading

Using pandas, the dataset is loaded into the app.

Step 2: Data Preprocessing

Text data like district names and monsoon phases are converted into numbers using Label Encoding.

Step 3: Model Building

A Random Forest Classifier is trained on historical weather data to predict weather labels.

Step 4: Feature Simulation

When the user selects a district and date, the system:

Calculates the day of the year.

Determines the monsoon phase.

Generates realistic temperature, humidity, and wind values for that district.

Step 5: Prediction

The model predicts the weather condition (like sunny, rainy, cloudy, etc.) for that input.

Step 6: Output Display

Results are shown interactively using Streamlit:

Selected district

Selected date

Predicted weather

Monsoon phase

Generated features (temperature, humidity, etc.)


 Model Used — Random Forest Classifier

Random Forest is an ensemble learning method that builds multiple decision trees and averages their results for better accuracy.

It works well for classification problems and is robust to noise.

Ideal for weather prediction due to its ability to handle both categorical and numerical data.


Implementation in Streamlit

The interface allows user input for district and date.

On clicking Predict, the app displays:

Monsoon phase

Generated environmental conditions

Predicted weather for the selected date

Output Example

Input:

District: Ernakulam

Date: 25 August 2025

Output:

Monsoon Phase: SouthWest Monsoon

Temperature: 28.5°C

Humidity: 84%

Predicted Weather: 🌧 Rainy


10. Applications

Smart Agriculture Systems for irrigation planning.

Tourism and Event Management to plan based on forecast.

Early Warning Systems for floods or heavy rain.

Local Government Planning for resource allocation.

Energy Management for solar/wind power forecasting.


Future Scope

Add real-time weather API integration for continuous updates.

Use deep learning (LSTM models) for time-series forecasting.

Include satellite and radar data for higher accuracy.

Deploy the app on cloud for public access.


Conclusion

The Kerala Smart Weather Predictor demonstrates how machine learning and data analysis can make weather forecasting smarter and more localized.
It’s a great example of how data-driven decision-making can help everyday life in agriculture, transport, and environmental planning.

