# car-sales-analysis
End-to-End Data analysis and Machine Learning Models for Car Sales Prediction

# Project Overview
The project was developed to advice and predict the selling price of used vehicles (foreign and local used) and brand new one for Nigerian automobile market. End-to-End industrial workflow was deployed in order to achieve optimum results. I started with data preprocessing and exploratory data analysis, model development, hyperparameter tuning, model evaluation, and price prediction for new vehicles.
The project objective is to provide the model that give best prediction to support data-driven decision for buyers and seller both retail or wholesale in Nigerian automobile market. Because of economic and political instability in Nigeria, the model should not be the only means of decision making in the automobile market arena.

# Project Objective
-	To develop and evaluate the best predicting model that can be used in selling vehicle.
-	To identify the factors that affect vehicle prices most.
-	To select and compare the performance of up to six regression models.
-	To develop a reusable preprocessing and prediction pipeline.
-	To enhance the selected model performance with the use of hyperparameter tuning.
-	To test the model to ascertain the percentage performance error and evaluate its application in the real world.
# Dataset
The dataset contains information on vehicles listed for sale in Nigeria.
Features include:
-	VehicleID
-	Location
-	Maker
-	Model
-	Year
-	Colour
-	Vehicle Type (Brand New, Foreign Used, Nigerian Used)
-	Distance (Mileage)
-	Vehicle Age (Engineered Feature)
Target Variable
-	Amount (Million Naira)

# Technologies Used
-	Python
-	Pandas
-	NumPy
-	Matplotlib
-	Scikit-learn
-	Joblib
-	Jupyter Notebook

# Project Workflow
Business Understanding<br>
	↓<br>
Data Collection
	↓<br>
Data Cleaning
	↓<br>
Missing Value Treatment
	↓<br>
Feature Engineering
	↓<br>
Exploratory Data Analysis
	↓<br>
Train-Test Split
	↓<br>
Preprocessing Pipeline
	↓<br>
Model Training
	↓<br>
Model Comparison
	↓<br>
Hyperparameter Tuning
	↓<br>
Model Evaluation
	↓<br>
Save Best Model
	↓<br>
Predict Selling Price


# End-to-End Industrial Workflow

# Data Preprocessing
The preprocessing stage included:
-	Missing value treatment
-	Data type correction
-	Standardization of categorical values
-	Feature engineering
-	Delivery mileage handling for brand-new vehicles
-	Vehicle age calculation
-	Building preprocessing pipeline with columnTransfomer

# Exploratory Data Analysis
-	Price distribution
-	Vehicle age distribution
-	Vehicle type distribution
-	Price by maker
-	Price by model
-	Price by location
-	Price versus mileage
-	Correlation among numerical variables

# Power BI
Power BI Dashboard
The interactive dashboard provides insights into transaction activity and fraud trends.

Executive KPIs
Dashboard Visualizations
Dashboard Preview






# Machine Learning Models
The following regression models were evaluated:
-	Linear Regression
-	Ridge Regression
-	Lasso Regression
-	Decision Tree Regressor
-	Random Forest Regressor
-	Gradient Boosting Regressor
  

# Model Performance	

|	Model				|	MAE		|	RMSE	|	R²Score		|	CVR²	
|-----------------------|-----------|-----------|---------------|------------
|	Random Forest		|	3.06	|	11.57	|	0.81		|	0.68
|						|			|			|				|
|	Gradient Boosting	|	4.49	|	12.26	|	0.79		|	0.68
|						|			|			|				|
|	Decision Tree		|	3.34	|	12.69	|	0.77		|	0.64
|						|			|			|				|
|	Ridge Regression	|	5.41	|	12.91	|	0.76		|	0.63
|						|			|			|				|
|	Linear Regression	|	6.29	|	14.00	|	0.72		|	0.56
|						|			|			|				|
|	Lasso Regression	|	7.89	|	22.51	|	0.28		|	0.30
|-----------------------|-----------|-----------|---------------|----------

# Best Performing Model
 Random Forest Regressor
Reasons:
-	Highest R² Score
-	Lowest MAE
-	Lowest RMSE
-	Best overall predictive performance

# Hyperparameter Tuning
The Random Forest model was further optimized using RandomizedSearchCV.
Optimized parameters included:
-	Number of trees
-	Maximum tree depth
-	Minimum samples split
-	Minimum samples leaf
This improved the robustness and generalization capability of the final model.

 # Sample Prediction
 
Example input: 

|	Feature 	|	Values	    |
|---------------|---------------|---
|	Location	|	Abuja
|---------------|---------------|---
|	Maker		|	Toyota
|---------------|---------------|----
|	Model		|	Camry
|---------------|---------------|----
|	Year		|	2023
|---------------|---------------|----
|	Colour		|	Black
|---------------|---------------|-----
|	Type		|	Brand New
|---------------|---------------|-
|	Distance	|	18 km
|---------------|---------------|-
|	Vehicle Age	|	1 year
|---------------|---------------|-

Predicted Selling Price:
₦77.15 Million

# Business Value
This solution is designed to support the following:
-	Vehicle dealers
-	Private buyers
-	Online vehicle dealers
-	Insurance companies
-	Financial institutions
Potential applications include:
-	Vehicle price prediction
-	Market trend analysis
-	Value of the vehicle
-	Price guide

Correlation Matrix
 
Correlation Matrix(Heat Map) Key
-	Dark Brown/Red (+1.0): Strong positive relationship ( as one goes up, the other goes up)
-	Dark Blue (-1.0): Strong negative relationship (as one goes up, the other goes down)
-	Grey (0.0): No relationship
Vehicle Price
-	Year vs. Price(+0.45): Brand new vehicles commands high vehicle price. Moderate positive relationship
-	Vehicle_age vs, Price(-0.45): As the vechile gets older, the price goes down. That why we have moderate negative
-	Distance vs. Price (-0.2): High mileage depreciates the Vehicle price.
Our main concern is on the vehicle price and we have realized that the year (new vehicle), vehicle age and mileage covered by the vehicle is the primary determinant of vehicle price

Actual vs. Predicted Prices
 
-	The red straight line graph with scattered plots presents perfect prediction
-	Any dot that falls directly on the line indicates that the model’s predicted price matched with the actual price.
Residual Plot
 
-	The Horizontal Axis (Predicted Price): This the  price estimates generated by your model.
-	The Vertical Axis (Residuals): This the error for each car prediction 
-	Residual = Actual Price - Predicted Price. 
o	0 Line (Red Dashed): Perfect predictions.
o	Above 0: Underestimation (the car actually sold for more than predicted).
o	Below 0: Overestimation (the car sold for less than predicted).
Please Note: For the scope of this project, no further improvement was carried out on the project.

Vehicle Age vs. Selling Price

 
-	The High-Variance Zone (0-5 Years): Brand new and lightly used vehicles show a massive spread in pricing. We have normal vehicles at the base, while the super luxury went up to the axis to 450 million Naira.
-	
-	The Steep Drop (6-15 Years): The maximum price dropped. At the year 10, even the most expensive vehicles managed to hit 250 million Naira. Which indicated that the most expensive vehicles loss their value fast in the last 10 years. 
-	
-	The Flatline (15+ Years): At the point a vehicle exceeds 15 years, the value depreciates. 
 Author
Bright C Egbuchulem
Data Analyst | Machine Learning Enthusiast | Civil Engineer
Technical Skills
-	Python
-	SQL
-	Power BI
-	Excel
-	Machine Learning
-	Predictive Analytics
-	Data Visualization
# Note 
This project was developed end-to-end machine learning as portfolio project to demonstrate practical skills in data preprocessing, predictive modelling, model evaluation by using Python and Scikit-learn.

One recommendation
This README is already at a strong academic and professional standard. To make it even more impressive for employers and admissions committees, I suggest adding:
•	Screenshots of your EDA plots.
•	A screenshot of your Power BI dashboard.
•	A short "Results at a Glance" section with the key metrics (R² = 0.81, MAE = 3.06, RMSE = 11.57).
•	Installation and usage instructions (git clone, pip install -r requirements.txt, and how to run the notebook).
Those additions will make your repository look polished and immediately useful to anyone reviewing it.

  	

