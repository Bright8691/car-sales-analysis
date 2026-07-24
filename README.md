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
**Power BI Dashboard**
<img width="720" height="420" alt="car-4_image" src="https://github.com/user-attachments/assets/8da64bc8-f83a-458b-bf5e-3d6d66c63fc2" />

The interactive dashboard provides insights into automobile sales.

**Dashboard Summary**<br>
The dashboard displays an executive overview of the automobile sales inventory across three major States in<br>
Nigerian automobile markets—Abuja, Lagos, and Ibadan. This will enable stakeholders to evaluate asset valuation,<br> differences in price, distribution of inventory, categories of automobile, and customer purchasing power.<br>
The dashboard further supports decision-making by helping dealerships understand where inventory is concentrated,<br> how vehicle values differ by location, and which customer price segments dominate the market.

**Executive KPIs**<br>
**Total Vehicles**<br>
7,205 Vehicles<br>
The dealership currently has 7,205 vehicles available for sale across all locations.<br>
Which is an evidence that the dealer having arrays of cars capable of serving across the multiple of customer groups.<br>

**Total Asset**<br>
₦85,259.47 Million<br>
The value equivalent in approximation to **₦85.26 billion**, in total assets of vehicles in the 3 locations. Which indicated that the dealer is prepared enough to satisfy the populace.<br>

**Average Car Price**<br>
₦11.83 Million<br>
This is the average cost of vehicles(Brand New, Foreign Used and Nigerian Used). It is for the purpose of know the average cost of vehicles. 

**Most Expensive Vehicle**<br>
₦456 Million<br>
The most expensive automobile is ₦456 million, which indicate that the dealer has vehciles across different classess in the society.

**Least Expensive Vehicle**<br>
₦0.45 Million<br>
The lowest vehicle price is approximately ₦450,000.00, far much below the average car price of ₦11.83 Million. This indicates the car hub is complete because it accommodates people from different working class.

**Visual Interpretation**

**1. Car Location Breakdown**<br>
This clustered column chart compares the distribution of Brand New, Foreign Used, and Nigerian Used vehicles across Lagos, Abuja, and Ibadan.<br>
**Insights**<br>
1. Lagos has the largest number of vehicles.
2. Foreign Used vehicles are in larger quantity in all locations because they are in high demand.
3. Brand New vehicles represent the smallest proportion of inventory because they are in low demand.
4. Nigerian Used vehicles contribute moderately to the available stock.<br>
**Business Value**
This helps the dealership in assets management and been aware where his assets is more concenrated.

**2. Inventory Valuation Matrix**<br>
This further shows each location's total monetry value by vehicle type

**Insights**
1. Abuja has more of Brand New and Luxury vehicles, as a result it has the highest inventory valuation.
2. This is followed by Lagos.
3. The smallest asset value is in Ibadan, because of lack in patronage.
   
**Business Value**
Helps the Management can identify where their capital is tied up and to prioritize investment.

**3. Listings by Location**<br>
The dashboard also provided the following reports:
1. Abuja Listings: 3,263
2. Lagos Listings: 3,318
3. Ibadan Listings: 624

**Insights**<br>
Lagos and Abuja account for the overwhelming majority of listings, while Ibadan has a comparatively smaller market presence.<br>
**Business Value**<br>
This gives an insight on how to support branch performance and furture plan to expansion the business.<br>
**4. Average Car Price by Location**<br>
**Insights**<br>
- The highest average sales were recorded in Abuja.
- This was followed by Lagos.
- Ibadan recorded the lowest average selling price.
**Business Value**<br>
This implies that Abuja has the highest purchacing power, followed by Lagos. There is need to have close monitoring of<br> sales in Abuja and Strategically improve sales in Ibadan.

**5. Customer Purchase Power by Volume**<br>
The donut chart segments customers into four price categories:
1. Budget (< ₦5M)
2. Mid-Range (₦5M–₦15M)
3. Premium (₦15M–₦30M)
4. Luxury (> ₦30M)
**Insights**<br>
The largest customer segment is the Budget category (about 43%), followed by Mid-Range (about 39%). Premium and Luxury buyers make up a much smaller share.
Business Value
The dealership should prioritize affordable and mid-range vehicles, as these segments account for the majority of demand.

**6. Price Segment by Year and Vehicle Type**<br>
This scatter plot visualizes the relationship between vehicle age, vehicle type, and price.
**Insights**
- Brand New vehicles generally occupy the higher price range.
- Foreign Used vehicles show moderate price variation.
- Nigerian Used vehicles are concentrated in the lower price segments.
**Business Value**
The visualization helps identify pricing patterns and market positioning across vehicle categories

**Slicers**<br>
The dashboard includes interactive filters for:
•	Vehicle Type
•	Price Segment
•	Location
These allow users to explore the dashboard dynamically based on their business needs.

**Business Insights**<br>
The analysis reveals that:
•	Lagos and Abuja dominate the Nigerian used-car market in terms of inventory and listings.
•	Abuja has the highest average vehicle price, indicating a stronger luxury market.
•	Foreign Used vehicles represent the largest portion of inventory.
•	Budget and Mid-Range vehicles account for more than 80% of customer demand, suggesting dealerships should prioritize stocking these categories.
•	Premium vehicles contribute significantly to total asset value despite representing a smaller proportion of inventory.

# Machine Learning Models<br>
The following regression models were evaluated:
1. Linear Regression
2. Ridge Regression
3. Lasso Regression
4. Decision Tree Regressor
5. Random Forest Regressor
6. Gradient Boosting Regressor
  

# Model Performance	

|	Model				|	MAE		|	RMSE	|	R²Score		|	CVR²	|	
|-----------------------|-----------|-----------|---------------|-----------|
|	Random Forest		|	3.06	|	11.57	|	0.81		|	0.68	|
|	Gradient Boosting	|	4.49	|	12.26	|	0.79		|	0.68	|
|	Decision Tree		|	3.34	|	12.69	|	0.77		|	0.64	|
|	Ridge Regression	|	5.41	|	12.91	|	0.76		|	0.63	|
|	Linear Regression	|	6.29	|	14.00	|	0.72		|	0.56	|
|	Lasso Regression	|	7.89	|	22.51	|	0.28		|	0.30	|


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


**Predicted Selling Price: ₦77.15 Million<br>Actual Selling Price: ₦75.00 million**


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


**Author: Bright C Egbuchulem<br>Data Analyst | Machine Learning Enthusiast | Civil Engineer**

**Technical Skills**
* **Python**
* **SQL**
* **Power BI**
* **Excel**
* **Machine Learning**
* **Predictive Analytics**
* **Data Visualization**

**Please Note**<br>This project was developed end-to-end machine learning as portfolio project to demonstrate<br>practical skills in data preprocessing, predictive modelling, model evaluation by using Python and Scikit-learn.


