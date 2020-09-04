# Classification of Asteroids

## Objective: 
The main objective of the project was to build a machine learning model that will classify if an asteroid is potential hazard or not for earth.

### Data Collection: 
* Data for this project was collected from Nasa's JPL small body database search engine in csv format that had aroud 900K+ entries.
* Url of the Nasa's JPL website [JPL small body database search engine] https://ssd.jpl.nasa.gov/sbdb_query.cgi#x
* It has 45 features and 995K entries.

### Data Preprocessing:
* Lots of features are dropped either bcz they had too many missing value or they were highly correlated.
* categorical variable also handled.
* feature scaling is also perform bcz many features values range vary too much.

### EDA:
* During this process it was seen that we have a imbalance data means skewed class.

### Model Selection: 
* For the imbalance data we used Random Forest classifier as our classification algorithm because it can handle imbalance data pretty well using class_weight hyperparameter.
* we desire high recall means of all the asteroid that are actually potential hazard what fraction did we actually detect correctly as potential hazard.
* This model gave us Recall=0.93 and accuracy=0.9886.

### Technologies Used:
* Python
* Jupyter Notebook
* Sklean
* RandomForest Classifier
* GridSearchCV
