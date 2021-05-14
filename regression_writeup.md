## Opening Gross Prediction
Sheralee Lovejoy

### Abstract
The purpose of this project is to help producers predict the opening gross of their movie. The gross opening weekend is crucial to the success of a movie and typically makes up about a third of the movie's entire domestic gross. Using data from Box Office Mojo, I created a prediction model based on numerical and categorical features to help producers get an idea of a reasonable budget range as well as the success of their movie.

### Design
For this project, data was collected from Box Office Mojo and focused on the “Top Lifetime Grosses” table. The table contains the top 1000 movies ranked by highest lifetime gross. Identifying features that have a strong relationship with opening gross will help determine what the potential success of the movie will be and how to incorporate that information with budgeting.

### Data
The dataset contains 1000 rows of movies each consisting 8 features, half of which are numerical and the other half categorical. A few feature highlights include budget, genre, and lifetime gross. 

### Algorithms
- Feature Engineering
- Converting categorical featured into dummy variables
- Scaling data

#### Models
After a comparison of Linear, RidgeCV, LassoCV, and LinearCV, I found that RidgeCV had the best validation and train score. However, due to the large discrepancy in scores, it was clear that the model was over fitting and needed some constraints.

#### Model Evaluation
The entire dataset was split into 3, 20% was set for the test holdout, 20% for validation, and 60% for training. Scores reported below were calculated with 5-fold cross validation on the test portion only.

#### Final Results: R^2 = 0.611 with RMSE = 2.4e+7

### Tools
BeautifulSoup, Selenium for web scraping
Pandas for data cleaning
Scikit-learn for modeling
Seaborn for heat map plotting