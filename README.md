# Sports Event Prediction Based on Online Sentiment

## Project Overview
I analyzed online sentiment from Reddit and ESPN to predict the outcomes of Major League Baseball (MLB) games. I leveraged web scraping, natural language processing (NLP), and machine learning to assess public opinion and make more informed sports betting decisions.

## Data Sources
The dataset is collected from Reddit and ESPN using web scraping and API calls.

## Objectives
- To collect and preprocess sentiment data from online sources.
- To analyze the impact of sentiment on sports outcomes using machine learning models.
- To provide actionable insights for sports betting.

## Methods
### Data Collection
- **Web Scraping**: Used Selenium and BeautifulSoup to scrape data from ESPN.
- **API Calls**: Used Reddit API to collect posts and comments.

### Data Processing
1. **Data Handling**:
   - Removed unnecessary columns and filtered data.
   - One-hot encoded categorical variables and handled missing values.

2. **Exploratory Data Analysis**:
   - Visualized data distributions and correlations.
   - Used histograms and scatter plots to identify patterns.

### Sentiment Analysis
- **NLP Processing**: Preprocessed text data by converting to lowercase and removing punctuation using NLTK.
- **Bag of Words Model**: Created a sentiment dictionary and calculated sentiment scores for text data.

### Machine Learning Models
1. **Lasso Regression**:
   - Used cross-validation to determine the optimal alpha parameter.
   - Trained the model with scaled data.

2. **Decision Tree**:
   - Built a decision tree with a maximum depth of 3 levels.
   - Trained the model without scaling the data.

3. **Random Forest**:
   - Built a random forest model.
   - Trained the model with scaled data.

## Results
### Lasso Regression
- Best alpha: 1.0
- MSE: 12,895,104,459,223.4
- RMSE: 3,590,975.42
- R-Squared: 0.4939

### Decision Tree
- MSE: 14,088,761,023,307.635
- RMSE: 3,753,499.84
- R-Squared: 0.4470

### Random Forest
- MSE: 9,534,609,658,387.262
- RMSE: 3,087,816.33
- R-Squared: 0.6258

## Recommendations
1. Refine the sentiment dictionary and improve labeling methods.
2. Expand the dataset to include more recent data and additional metrics.
3. Explore advanced modeling techniques and fine-tune existing models.

## Conclusion
The Random Forest model was the most effective in predicting MLB game outcomes based on online sentiment, explaining 62.6% of the variance. Future work will focus on refining the models and expanding the dataset for better accuracy.

