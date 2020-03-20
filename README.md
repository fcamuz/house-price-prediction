
# The King County Housing Price Prediction Model¶

In this project I did EDA(Exploratory Data Analysis) to get insight from the data and created a model to predict the house pricing in King County. 

### Methodology:

In this project I will follow the OSEMN process to solve a problem and create a model to predict the house pricing in King County. OSEMN is an acronym that represents Obtain, Scrub, Explore, Model, and iNterpret steps.  

### Dataset:

Kings County Data Set from Kaggle

Column Names and descriptions 
id - unique identified for a house
date - Date house was sold
price - Price is prediction target
bedrooms - Number of Bedrooms/House
bathrooms - Number of bathrooms/bedrooms
sqft_living - square footage of the home
sqft_lot - square footage of the lot
floors - Total floors (levels) in house
waterfront - House which has a view to a waterfront
view - Has been viewed
condition - How good the condition is ( Overall )
grade - overall grade given to the housing unit, based on King County grading system
sqft_above - square footage of house apart from basement
sqft_basement - square footage of the basement
yr_built - Built Year
yr_renovated - Year when house was renovated
zipcode - zip
lat - Latitude coordinate
long - Longitude coordinate
sqft_living15 - The square footage of interior housing living space for the nearest 15 neighbors
sqft_lot15- The square footage of the land lots of the nearest 15 neighbors


### Model:
Linear Regression Model


### Conclusion :

This model can make  **81%** accurate prediction for a house price

#### Features that go through the model are;

Location (latitude and longitude)
Number of bedrooms
Living, lot and basement size
Number of views the house get
Year of built
Number of floors
Condition

#### Most significant features are;

Location, condition, living area and waterfront effects a house price more than any other features.

#### How does that work?
Each features effect the model result based on their coefficents. Coefficient define how many unit a feature change the target as it increase one unit. According to this model;

Latitude and longitude ~ upto 1.46 unit)
Condition grade higher than 3 ~ (3 :0.8 unit, 4: 0.9 unit, 5:1.0 unit,)
View (the most significant view is waterfront ~ 0.63 unit
Living area size ~ 0.48 unit

#### Findings
Larger lots does not increase the price of a house directly. But the larger house size always increase the house price. Choose Seattle, East Urban and East Rural areas to built houses. Always keep the living area large. Keep the lot size minimum in Seattle and East Urban area. Built relatively larger lots in South Urban, west of East Rural and west of South Rural area. Have options for huge lots for farm houses in the east side of the county.

#### Future Work
A price comparison can be done for per sqft of house and lot size to make better decision when splitting the land into living and lot area. Also another model can be created to give best split percentages to get maximum price by the zipcode of the land.