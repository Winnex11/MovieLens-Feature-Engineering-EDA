# MovieLens Feature Engineering & Exploratory Data Analysis

## Project Overview
This project focuses on cleaning, exploring, and performing feature engineering on the MovieLens dataset to uncover meaningful insights about movie ratings, genre popularity, and user behavior. The analysis demonstrates how engineered features and exploratory analysis can support the design of a future movie recommendation system.

## Dataset
- **Source:** MovieLens (GroupLens Research)
- **Files Used:** ratings.csv, movies.csv, tags.csv, links.csv
- **Description:**  
The dataset contains user ratings, movie metadata, genres, user-generated tags, and external references (IMDb and TMDb), enabling detailed analysis of movie trends and audience preferences.

Dataset link:  
https://grouplens.org/datasets/movielens/

## Tools & Libraries
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

## Data Preparation
The following steps were carried out:
- Loaded and merged all datasets using the `movieId` key.
- Checked for and removed duplicate records.
- Verified missing values.
- Converted timestamp columns into proper datetime format to enable time-based analysis.

This resulted in a unified and clean dataset suitable for feature engineering and exploration.

## Feature Engineering
The following features were created to enrich the dataset:

- **Release Year** – Extracted from movie titles to analyze trends across different time periods.
- **Genre Count** – Number of genres associated with each movie to study genre diversity effects.
- **Average Rating per Movie** – Used to rank movies based on viewer satisfaction.
- **Average Rating per Genre** – Helps identify genres that audiences rate more favorably.
- **Number of Ratings per Genre** – Indicates genre popularity and user engagement.
- **Rating Year** – Extracted from timestamps to analyze how rating activity changes over time.

These features are useful for improving personalization and relevance in recommendation systems.

## Exploratory Data Analysis (EDA)
Key analyses performed include:
- Distribution of movie ratings
- Comparison of average ratings across genres
- Identification of the most and least watched genres
- Analysis of rating activity trends over time
- Examination of average movie ratings by year

## Key Insights
- Movie ratings are skewed toward higher values, with most users rating movies between 4.0 and 5.0.
- Drama and Crime genres consistently receive the highest average ratings.
- Popular genres such as Drama, Comedy, Action, and Thriller dominate user engagement.
- Niche genres like Film-Noir, Western, and Documentary receive fewer ratings, reflecting smaller but loyal audiences.
- User rating activity has increased over time, likely due to the growth of online platforms and streaming services.
- Average movie ratings fluctuate over the years, indicating changing audience preferences and industry trends.

## Recommendation System Relevance
The insights and engineered features from this analysis can support:
- Cold-start recommendations for new users
- Genre-based personalization
- Time-aware recommendation strategies
- Improved understanding of evolving user preferences

## Limitations
- Ratings data may exhibit positivity bias, as users tend to rate movies they already like.
- Some genres have significantly fewer ratings, which may affect statistical reliability.
- The dataset does not include detailed user demographic information.

## Future Work
- Incorporate collaborative filtering techniques.
- Apply machine learning models for rating prediction.
- Integrate additional user behavior and demographic data.
- Build interactive dashboards to visualize recommendation insights.

## Links
- Dataset source: https://grouplens.org/datasets/movielens/
