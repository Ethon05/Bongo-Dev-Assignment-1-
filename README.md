# Bongo-Dev-Assignment-1-
Netflix Dataset Analysis and Preprocessing  This project explores and preprocesses the Netflix dataset to prepare it for machine learning tasks. It includes data loading, cleaning, exploratory data analysis (EDA), and feature engineering.
## Overview

The `netflix_analysis.ipynb` notebook details the following steps:

1.  **Data Loading and Initial Inspection:** Loading the `netflix_titles.csv` file using pandas and examining the first and last few rows, as well as general information about the dataset.
2.  **Data Cleaning:** Addressing missing values in columns like `director`, `cast`, and `country` using appropriate strategies.
3.  **Exploratory Data Analysis (EDA):**
    * Visualizing the distribution of content types (Movies vs. TV Shows).
    * Analyzing trends in content addition over time.
    * Identifying and handling outliers in the `release_year` column.
    * Determining the top content-producing countries.
4.  **Feature Engineering:**
    * Extracting numerical values from the `duration` column to separate the number and the unit (minutes or seasons).
    * Preparing categorical features for machine learning (though specific encoding methods might depend on the downstream task).
5.  **Data Splitting (Conceptual):** The notebook outlines the intention to split the data into training, validation, and testing sets, a crucial step for machine learning model development.

## Libraries Used

The following Python libraries were used in this project:

* pandas
* numpy
* seaborn
* matplotlib.pyplot
* scikit-learn (`sklearn`)
* scipy.stats

## Dataset

The dataset (`netflix_data.csv`) contains information about movies and TV shows available on Netflix. Each row represents a title, and the columns include:

* `show_id`: Unique identifier for each show.
* `type`: Whether it's a Movie or a TV Show.
* `title`: The title of the movie or show.
* `director`: The director(s) of the movie or show.
* `cast`: The main actors and actresses.
* `country`: The country or countries where the content was produced.
* `date_added`: The date when the title was added to Netflix.
* `release_year`: The year the movie or show was released.
* `rating`: The content rating (e.g., TV-MA, PG-13).
* `duration`: The length of the movie (in minutes) or the number of seasons for a TV show.
* `listed_in`: The genres the title is categorized under.
* `description`: A brief summary of the content.

## Potential Future Work

* Implement specific machine learning models (e.g., recommendation systems).
* Perform more advanced feature engineering on text data (title, description, cast, director, listed\_in).
* Deploy the preprocessed data or a trained model.
