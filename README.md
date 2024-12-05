# Yelp Restaurant Sentiment Analysis and Geographic Trends
This project explores **customer sentiment** and **geographic trends** in Yelp reviews across three distinct restaurant categories: Breakfast & Brunch, Pizza, and Specialty Food. By leveraging the Yelp dataset, this study investigates how geographic location impacts restaurant performance and customer satisfaction.

## Table of Contents
## Overview
Yelp has transformed how customers evaluate dining options, providing a robust dataset to analyze restaurant performance and customer preferences. This project focuses on three restaurant categories:

- Breakfast & Brunch: Known for its time-sensitive appeal and social dining experiences.
- Pizza: A highly competitive and universally loved category.
- Specialty Food: Reflecting trends in health-conscious dining, such as vegan and gluten-free options.
  
Using advanced data analysis techniques, this study identifies trends in restaurant performance and customer satisfaction across major metropolitan areas in the United States and Canada.

## Technologies
This project utilizes the following technologies:

- **Python** for data analysis and visualization
- **Pandas** and **NumPy** for data processing
- **GeoPandas** and **SEDAC** for geospatial analysis
- **VADER** for sentiment analysis
- **DBSCAN** and **K-Means Clustering** for pattern identification
- **Matplotlib** and **Seaborn** for visualization

## Methodology
### Data Acquisition
The Yelp dataset, available on Kaggle, includes:
- Reviews
- Business information
- User profiles
- Tips
- Check-ins
This dataset covers businesses across eight major metropolitan areas in North America.

### Data Cleaning
Data preprocessing was critical to ensure accuracy and reliability:
- Missing values in geographic coordinates, ratings, and reviews were filtered out.
- Text normalization involved converting strings to lowercase and splitting multi-category entries.
- Outliers were handled to prevent skewed results.

### Clustering and Geographic Analysis
To identify regional patterns in restaurant performance, the following clustering techniques were applied:

- K-Means Clustering to group businesses by average star ratings, review counts, latitude, and longitude.
- DBSCAN to detect density-based patterns and outliers.

### Sentiment Analysis
The VADER (Valence Aware Dictionary and sEntiment Reasoner) tool was used to classify sentiments in Yelp reviews:

- Positive sentiment: VADER scores > 0.05
- Neutral sentiment: VADER scores between -0.05 and 0.05
- Negative sentiment: VADER scores < -0.05
Sentiment scores were analyzed to uncover regional and categorical trends.

## Results
### Key Insights
High-Performing Clusters:
- Cluster 2 (Northern Mississippi/Alabama): Average Rating: 4.13
- Cluster 4 (Las Vegas, NV): Average Rating: 3.65
  
Geographic Trends:
- Urban areas displayed more balanced sentiment distributions.
- Rural areas exhibited sentiment extremes.

Category-Specific Findings:
- Breakfast & Brunch: Temporal sentiment variations were observed, with weekends showing higher positivity.
- Pizza: Most consistent sentiment correlations across all regions.
- Specialty Food: High variability in sentiment, reflecting niche customer expectations.

### Visualizations
- Sentiment distributions for high- and low-performing businesses
- Geographic clustering results
- Temporal sentiment trends for Breakfast & Brunch

## Limitations and Future Work
### Limitations
- Sparse data: Limited reviews from Canadian provinces restricted the generalizability of findings in Canada.
- Sentiment analysis limitations: VADER may miss deeper contextual meanings in review text.
- Focus on three categories: Expanding to additional restaurant categories would provide a more comprehensive analysis.

### Future Work
- Incorporate advanced sentiment analysis tools, such as BERT, to improve accuracy.
- Expand the dataset to include a broader geographic and categorical scope.
- Explore additional dining categories for a deeper understanding of customer preferences.

## Authors
Wanjing (Anna) Yan
- Master's Student, Big Data Analytics, San Diego State University
- Email: wyan4786@sdsu.edu

Maedeh Rahimi
- Master's Student, Hydrology, San Diego State University
- Email: mrahimimashkel1705@sdsu.edu

Nadjim Noori
- Master's Student, Information Processing, University of Cologne
- Email: nnoori7150@sdsu.edu
  
## References
- Asghar, N. (2016). Yelp dataset challenge: Review rating prediction. arXiv preprint arXiv:1605.05362.
- Carbon, K., Fujii, K., & Veerina, P. (2014). Applications of Machine Learning to Predict Yelp Ratings. Stanford University.
- Hutto, C., & Gilbert, E. (2014, May). Vader: A parsimonious rule-based model for sentiment analysis of social media text. In Proceedings of the international AAAI conference on web and social media (Vol. 8, No. 1, pp. 216-225).
- Kharde, V., & Sonawane, P. (2016). Sentiment analysis of Twitter data: a survey of techniques. arXiv preprint arXiv:1601.06971.
- Singh, M., Jakhar, A. K., & Pandey, S. (2021). Sentiment analysis on the impact of coronavirus in social life using the BERT model. Social Network Analysis and Mining, 11(1), 33.
- Talaat, A. S. (2023). Sentiment analysis classification system using hybrid BERT models. Journal of Big Data, 10(1), 110.
- Yelp Inc. (2024). Yelp dataset (Version 1) [Data set]. Kaggle. https://www.kaggle.com/datasets/yelp-dataset/yelp-dataset

