# fordgobike-tripdata-EDA
Exploratory Data Analysis (EDA) on Ford GoBike Trip Data
Project Overview
This project performs Exploratory Data Analysis (EDA) on the Ford GoBike trip data collected in February 2019. The dataset includes information about bike trips taken by users, with attributes such as trip duration, start and end times, start and end stations, and user details (age, gender, and user type). The goal of this analysis is to gain insights into various factors such as trip duration, user demographics, and trends in bike usage across different user types and age groups.

Dataset Description
The dataset, 201902-fordgobike-tripdata.csv, consists of the following columns:

duration_sec: Duration of the trip in seconds.
start_time: Start time of the trip.
end_time: End time of the trip.
start_station_id: ID of the station where the trip started.
start_station_name: Name of the station where the trip started.
start_station_latitude: Latitude of the start station.
start_station_longitude: Longitude of the start station.
end_station_id: ID of the station where the trip ended.
end_station_name: Name of the station where the trip ended.
end_station_latitude: Latitude of the end station.
end_station_longitude: Longitude of the end station.
bike_id: ID of the bike used.
user_type: Type of user (Customer or Subscriber).
member_birth_year: Birth year of the user.
member_gender: Gender of the user.
bike_share_for_all_trip: Whether the trip was part of the bike-share program.
Goals of the Exploration
The main goals of this analysis are:

Data Cleaning: Handling missing values and irrelevant columns.
Demographic Analysis: Investigating how age, gender, and user type affect trip duration and frequency.
Duration Analysis: Understanding trip duration trends and identifying any outliers.
Exploring User Behavior: Analyzing the distribution of users by age, gender, and user type.
Key Insights
Age Distribution:

Users were grouped into age categories such as very young, young, midlife, old, and very old based on their birth year.
The majority of users fall within the midlife and old age groups.
User Type:

There are two main user types: Customer and Subscriber.
Subscribers tend to have shorter trips on average compared to customers.
Trip Duration:

The average trip duration is 726 seconds, with a large spread (ranging from a few seconds to over 20 hours). This suggests that some trips may be outliers and should be treated separately.
Gender Distribution:

Male users account for the majority of the trips, followed by Female users. Other genders are less represented.
Most Frequent Trip Times:

The dataset includes timestamps for each trip, and the majority of trips are taken during the afternoon and evening hours.
Visualizations
The project includes several visualizations to understand the dataset better:

Box Plots: For analyzing the distribution of trip durations and birth years.
Histograms: To show the distribution of users' ages.
Pie Charts: To represent the proportion of users in different age groups and user types.
Scatter Plots: To visualize the relationship between age groups and trip duration.
Count Plots: To visualize the distribution of categorical variables like age group, gender, and user type.
Data Cleaning and Transformation
Handling Missing Values: Missing values in the member_birth_year and member_gender columns were filled with the mean of member_birth_year and left NaN in member_gender for users without gender data.
Feature Engineering: The member_birth_year was converted into age groups (AgeGroup) for easier analysis.
Technologies Used
Python: Main programming language.
Pandas: For data manipulation and analysis.
Matplotlib & Seaborn: For creating visualizations.
NumPy: For numerical operations and handling large datasets.
Scikit-learn: For generating classification reports and confusion matrices.
How to Use
Clone the repository:
bash
Copy code
git clone https://github.com/your-username/ford-gobike-eda
cd ford-gobike-eda
Install the required dependencies:
bash
Copy code
pip install -r requirements.txt
Run the EDA:
bash
Copy code
jupyter notebook FordGoBike_EDA.ipynb
This will open the Jupyter notebook where you can explore the analysis, visualizations, and insights.
Future Work
Predicting Trip Duration: Using machine learning to predict trip duration based on user demographics, start/end stations, etc.
User Behavior Prediction: Understanding the relationship between user type and behavior, potentially predicting whether a user will subscribe based on their trip patterns.
Seasonal and Time Analysis: Exploring how seasonality (months, weather) affects the usage of bikes.
Results
This analysis offers valuable insights into the usage patterns of the Ford GoBike system. By analyzing various aspects of the data, we can better understand how users interact with the bike-sharing service, which can guide future improvements.

