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
Data Collection<br>
	↓<br>
Data Cleaning<br>
	↓<br>
Missing Value Treatment<br>
	↓<br>
Feature Engineering<br>
	↓<br>
Exploratory Data Analysis<br>
	↓<br>
Train-Test Split<br>
	↓<br>
Preprocessing Pipeline<br>
	↓<br>
Model Training<br>
	↓<br>
Model Comparison<br>
	↓<br>
Hyperparameter Tuning<br>
	↓<br>
Model Evaluation<br>
	↓<br>
Save Best Model<br>
	↓<br>
Predict Selling Price<br>


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

Executive KPIs<br>
Dashboard Visualizations<br>
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


# Best Performing Model
**Random Forest Regressor**
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
 
**Example input:** 

|	Feature 	|	Values	    |
|---------------|---------------|
|	Location	|	Abuja
|				|
|	Maker		|	Toyota
|				|
|	Model		|	Camry
|				|
|	Year		|	2023
|				|
|	Colour		|	Black
|				|
|	Type		|	Brand New
|				|
|	Distance	|	18 km
|				|
|	Vehicle Age	|	1 year


**Predicted Selling Price:**
**₦77.15 Million**

# Business Value
This solution is designed to support the following:
-	Vehicle dealers
-	Private buyers
-	Online vehicle dealers
-	Insurance companies
-	Financial institutions<br>
Potential applications include:
-	Vehicle price prediction
-	Market trend analysis
-	Value of the vehicle
-	Price guide


**Correlation Matrix**<br>

<img width="400" height="350" alt="20260722_170641" src="https://github.com/user-attachments/assets/555d73b5-5e51-412a-b1f0-a162cb546040" /><br>
 
Correlation Matrix(Heat Map) Key
-	Dark Brown/Red (+1.0): Strong positive relationship ( as one goes up, the other goes up)
-	Dark Blue (-1.0): Strong negative relationship (as one goes up, the other goes down)
-	Grey (0.0): No relationship
Vehicle Price
-	Year vs. Price(+0.45): Brand new vehicles commands high vehicle price. Moderate positive relationship
-	Vehicle_age vs, Price(-0.45): As the vechile gets older, the price goes down. That why we have moderate negative
-	Distance vs. Price (-0.2): High mileage depreciates the Vehicle price.
Our main concern is on the vehicle price and we have realized that the year (new vehicle), vehicle age and mileage covered by the vehicle is the primary determinant of vehicle price

**Actual vs. Predicted Prices**<br>

<img width="400" height="350" alt="20260722_172655" src="https://github.com/user-attachments/assets/1232e26f-70a0-4dc7-bc87-52cd296e3c92" />

 
-	The red straight line graph with scattered plots presents perfect prediction
-	Any dot that falls directly on the line indicates that the model’s predicted price matched with the actual price.

**Residual Plot**<br>

<img width="400" height="350" alt="20260722_172556" src="https://github.com/user-attachments/assets/88abe13a-90bc-4fff-b59c-c581d216e0c3" /><br>

 -	The Horizontal Axis (Predicted Price): This the  price estimates generated by your model.
-	The Vertical Axis (Residuals): This the error for each car prediction 
-	Residual = Actual Price - Predicted Price. 
-	0 Line (Red Dashed): Perfect predictions.
-	Above 0: Underestimation (the car actually sold for more than predicted).
-	Below 0: Overestimation (the car sold for less than predicted).

Please Note: For the scope of this project, no further improvement was carried out on the project.

**Vehicle Age vs. Selling Price**<br>

<img width="400" height="350" alt="20260722_171355" src="https://github.com/user-attachments/assets/9df7c45e-2724-49db-8a56-a72e10fede7c" /><br>

 -	The High-Variance Zone (0-5 Years): Brand new and lightly used vehicles show a massive spread in pricing. We have normal 	vehicles at the base, while the super luxury went up to the axis to 450 million Naira.
-	The Steep Drop (6-15 Years): The maximum price dropped. At the year 10, even the most expensive vehicles managed to hit 	250 million Naira. Which indicated that the most expensive vehicles loss their value fast in the last 10 years. 
-	The Flatline (15+ Years): At the point a vehicle exceeds 15 years, the value depreciates. 


**Author**
**Bright C Egbuchulem**
**Data Analyst | Machine Learning Enthusiast | Civil Engineer**

**Technical Skills**
* **Python**
* **SQL**
* **Power BI**
* **Excel**
* **Machine Learning**
* **Predictive Analytics**
* **Data Visualization**

**Please Note**<br> 
This project was developed end-to-end machine learning as portfolio project to demonstrate practical skills in data preprocessing, predictive modelling, model evaluation by using Python and Scikit-learn.


