# Final-Project-Statistical-Modelling-with-Python

## Project/Goals

The project goal is to compare and analyze the APIs of both Foursquare and Yelp.  Using statistical modeling  to find deeper findings between bike stations and the density/popularity of restaurants in a very small and specific radius. 

- Using the APIs and where they cover in a 1000M radius between them
- Finding appropriate relationships between restaurants and bike stations.
- Using statistical modeling to predict bike availability based on ratings and bike station counts.

## Process

1. Data/API Analysis
- Utilized the Yelp and Foursquare APIs to extract and explore data on bike stations and restaurant ratings.
- Conducted a thorough analysis of the obtained data, gaining insights into the features and characteristics of bike stations and restaurant ratings, contributing to a comprehensive understanding of the urban landscape.
3. Data Validation and Preparation
- Conducted a meticulous examination of each dataset to identify and address missing or inconsistent data.
- Utilized both queries and visualization tools to scrutinize the structure, columns, and data types of the Yelp and Foursquare datasets, leading to informed decisions on cleaning, dropping unnecessary columns, filling null values, and removing zeros for enhanced data quality.
4. Statistical Modelling
- Explored the relationships among key variables such as 'rating', 'review_count', 'free_bikes', and 'distance' to identify potential correlations.
- Delved into the impact of restaurant ratings on the presence of free bikes through comprehensive regression analysis.
- Applied Ordinary Least Squares (OLS) regression to forecast the availability of free bikes, focusing on essential factors like 'rating' and 'bike_station'.

## Results
API Comparison:

- Yelp outperformed Foursquare in terms of data accessibility and utility, particularly in response to backend requests. Despite having more extraneous information, Yelp's core data components surpassed Foursquare in overall quality and usefulness.
- The Yelp API delivered a more extensive dataset, incorporating essential details like restaurant names, image URLs, operational status, user reviews, categorized information, ratings, and detailed location specifics. The emphasis on user-generated reviews within Yelp's dataset contributed to a more nuanced and precise portrayal of restaurant quality and popularity when compared to Foursquare.

Statistical Modelling
F-Statistic and Heteroscedasticity Test:

F-Statistic: The p-value for the F-statistic is 0.0709, suggesting that we lack sufficient evidence to reject the null hypothesis. This supports the conclusion that there is no strong indication of heteroscedasticity in the residuals.
Adjusted R-squared: The adjusted R-squared of 0.071 indicates that approximately 12.4% of the variability in 'rating' is explained by the independent variables. It is adjusted for the number of irrelevant variables in the model.
Correlation Analysis:

Positive Correlation: Found a moderate positive correlation between the number of free bikes and restaurant ratings, implying a tendency for higher-rated restaurants to have more available free bikes.
Customer Behavior: The more free bikes available, the higher the likelihood of customers renting a bike and leaving it in the area, contributing to the station's bike count. Or, there's the likelihood of being higher bike stations available around higher-end neighborhoods could be due to those neighborhoods being less likely to use or own bikes as their means of transportation

## Challenges 
- Data Quality Challenges:

Missing or Inconsistent Data: Faced challenges in handling missing or inconsistent data within API responses, requiring careful data cleaning and preprocessing.
Multicollinearity Concerns: Addressing potential multicollinearity issues in the regression model posed a challenge, emphasizing the need for feature selection and model refinement.
Data Integration Challenges:

Data Joining and Merging: Merging data from different APIs based on common columns presented challenges, requiring a systematic approach to ensure accurate integration.
Interpretation Challenges:

Subtle Relationships: Interpreting subtle relationships between variables due to weak correlations demanded a nuanced understanding of the data, prompting the exploration of alternative models and data points.
Visualization and Model Selection Challenges:

Data Representation: Difficulty in effectively representing data through graphs may have hindered a comprehensive understanding. Exploring more suitable visualizations could enhance the presentation of findings.
Model Exploration: Exploring different models and data points could provide insights into which hypotheses to pursue, potentially refining the analysis and uncovering more meaningful patterns.
## Future Goals
Incorporate Additional Variables:

Explore and integrate more relevant variables or datasets that might contribute to a more comprehensive understanding of bike station dynamics and their relationship with restaurant ratings. This could involve factors such as weather conditions, traffic patterns, or local events, which might influence both bike usage and restaurant popularity.
In-Depth Analysis of User Reviews:

Dive deeper into user reviews from platforms like Yelp to uncover patterns or sentiments that could provide richer insights into the dynamics between bike stations and restaurant ratings. This could involve sentiment analysis or topic modeling to extract valuable information from textual data and understand the qualitative aspects of user experiences.
Geospatial Analysis:

Implement geospatial variables, including distance and specific location details, into the regression model. This could help uncover spatial patterns and relationships between bike station availability and the geographical distribution of restaurants. Understanding how proximity and spatial factors impact bike station dynamics could add a valuable layer to the analysis.
Model Refinement and Validation:

Further refine the regression model by addressing potential issues such as multicollinearity and outliers. Additionally, consider employing more advanced modeling techniques or machine learning algorithms to assess their performance in predicting bike station availability based on restaurant ratings. Model validation through techniques like cross-validation could provide a more robust evaluation of the model's generalizability.
