Delivery Time Prediction Using Linear Regression
Project Overview
This project aims to predict the time taken for a delivery based on various features such as the type of vehicle, type of order, distance, and weather conditions. The dataset is processed, cleaned, and analyzed using pandas, and the prediction is made using a Linear Regression model from the scikit-learn library. The model's performance is evaluated using metrics such as Mean Squared Error (MSE) and R² score.

Dataset
The dataset contains the following columns:

ID: Identifier for each delivery (dropped during preprocessing).
Delivery_person_ID: Identifier for the delivery person (dropped during preprocessing).
Delivery_person_Age: Age of the delivery person.
Delivery_person_Ratings: Ratings given to the delivery person.
Distance: Distance to the delivery location.
Weather_conditions: Weather conditions at the time of delivery.
Road_traffic_density: Road traffic density during the delivery.
Type_of_order: Type of order (e.g., Food, Groceries, etc.).
Type_of_vehicle: Type of vehicle used for delivery (e.g., Bike, Car, etc.).
Multiple_deliveries: Whether the delivery person was handling multiple deliveries at the time.
Festival: Whether there was a festival during the delivery period.
City: City of the delivery.
Time_taken(min): Target variable representing the time taken for delivery in minutes.
Workflow
Data Preprocessing:

Drop the ID and Delivery_person_ID columns as they are not useful for the prediction.
Rename the column Time_taken(min) to Time_taken for easier usage.
Encode categorical variables such as Type_of_order and Type_of_vehicle using LabelEncoder to convert string values into numerical ones.
Exploratory Data Analysis (EDA):

Create bar plots and box plots to visualize how the delivery time varies based on the type of vehicle and type of order.
Identify if any columns contain missing or null values.
Model Training:

The dataset is split into training and test sets using an 80-20 split.
Train a Linear Regression model using the training set.
Model Prediction:

Predict the delivery time for a given set of features (e.g., vehicle type, order type, distance, etc.).
Evaluate the model using Mean Squared Error (MSE) and R² score on the test set.
