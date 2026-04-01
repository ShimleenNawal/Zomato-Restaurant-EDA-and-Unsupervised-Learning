# Zomato-Restaurant-EDA-and-Unsupervised-Learning

## Project Overview

This project focuses on analyzing Zomato restaurant data to uncover meaningful insights about customer preferences, restaurant performance, and pricing strategies. It combines **Exploratory Data Analysis (EDA), Natural Language Processing (NLP), and Machine Learning models** to derive actionable business insights.

## Business Objective

The objective of this project is to help restaurants and food platforms:

- Understand customer behavior and satisfaction
- Identify key factors influencing ratings
- Segment restaurants based on performance
- Improve decision-making using data-driven insights

## Dataset Description

The project uses two datasets:

**1. Restaurant Metadata**
- Name
- Cost (per person in ₹)
- Cuisines
- Collections
- Timings
  
**2. Customer Reviews**
- Restaurant
- Reviewer
- Review Text
- Rating
- Metadata
- Time
  
## Data Preprocessing
- Handled missing values using appropriate strategies
- Cleaned inconsistent and noisy data
- Converted data types
- Treated outliers using IQR method
- Extracted features such as review length
  
## Feature Engineering
- Text preprocessing:
  - Lowercasing
  - Removing punctuation, URLs, and stopwords
  - Tokenization and lemmatization
- Sentiment analysis:
  - Extracted sentiment polarity using TextBlob
- Created new features:
  - Cost categories
  - Review length
  - Rating classes
  
## Exploratory Data Analysis (EDA)

Performed structured analysis using:

- Univariate Analysis
- Bivariate Analysis
- Multivariate Analysis
  
## Key Insights:
- Majority of restaurants fall in the mid-price range
- Ratings are skewed toward higher values
- Certain cuisines dominate the market
- Review length has no significant impact on ratings
  
## Hypothesis Testing
Tested relationships between:
- Cost and Rating
- Review Length and Rating
- Cost Category and Rating
  
## Findings:
- No strong relationship between review length and rating
- Pricing has limited direct influence on customer satisfaction
  
## Machine Learning Models
**1. KMeans Clustering**
- Segmented restaurants based on cost, rating, and sentiment
- Evaluated using Silhouette Score
  
**2. Random Forest Regressor**
- Predicted continuous ratings
- Evaluated using:
  - R² Score
  - RMSE
    
**3. Logistic Regression (Final Model)**
- Classified ratings into:
  - Low
  - Medium
  - High
- Achieved:
  - Accuracy: 74.3%
  
## Final Model Selection

Logistic Regression was selected because:

- Provides interpretable classification outputs
- Aligns better with business decision-making
- Enables identification of low-performing restaurants
  
## Dimensionality Reduction
- Applied PCA
- Retained ~75% variance using 2 components
- Used for visualization and pattern recognition
  
## Business Insights
- Customer satisfaction depends more on experience than pricing
- Sentiment analysis provides deeper understanding of feedback
- Restaurants can use segmentation to improve performance
- Classification models help identify high-risk and high-performing segments

## Conclusion

This project demonstrates how combining EDA, NLP, and machine learning can transform raw restaurant data into actionable insights. The findings can help improve customer experience, optimize pricing strategies, and support data-driven decision-making.

## Tech Stack
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- NLTK, TextBlob
