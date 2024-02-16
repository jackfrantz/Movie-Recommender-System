# Movie Recommender System

## Overview
This project aims to analyze movie review data with the end goal being to create a recommender system that can recommend movies based on movie ratings from other users that like similar movies to the ones searched in the recommender system.

## Problem Statement
I have been tasked by a start-up company that aims to help movie lovers find new content. 

## Analysis

## Data
Due to storage constrictions, the majority of data for this project is not stored on GitHub. The source data and additional data files created throughout the project were masked from GitHub using a folder called `Large-Data` that is included in the .gitignore file. The links for the data sets used are listed below.

- [MovieLens](https://grouplens.org/datasets/movielens/): MovieLens 25M Dataset
- [IEEE](https://ieee-dataport.org/open-access/imdb-users-ratings-dataset): IMDb User Ratings Dataset
- [IMDb Non-Commercial Datasets](https://developer.imdb.com/non-commercial-datasets/): IMDb title.akas.tsv.gz Dataset
- [Kaggle](https://www.kaggle.com/datasets/rounakbanik/the-movies-dataset?select=movies_metadata.csv): The Movie Dataset

### Languages and Libraries Used
- Languages
    - Python
- Libraries
    - Data Analysis
        - Pandas
        - NumPy
    - Visualization
        - Matplotlib
        - Seaborn
    - Modeling
        - SciPy
        - Sklearn

### Visualizations

The following visualizations are included in this project:

1. Distributions of movie rating score by users from MovieLens and IMDb.
2. Top-rated and worst-rated movies overall.
3. Distributions of the number of reviews per movie.

## Files and Directory Structure
- Code_Notebooks
    - `1_Data_Collection.ipynb`: Jupyter Notebook containing the code for reading in and formatting the source dat.
    - `2_Data_Cleaning.ipynb`: Jupyter Notebook containing code for cleaning and formatting datasets to prepare for EDA and Modeling.
    - `3_EDA.ipynb`: Jupyter Notebook containing containing the exploratory data analysis and code for generating the visualizations that were used in the slide deck for presentation.
    - `4_Modeling.ipynb`: Jupyter Notebook containing the code for constructing a recommender system using the movie review datasets that were prepared during data cleaning
- Data
    - `movies.csv`: This dataset contains the movies that were included in the MovieLens 25M dataset. It can be used to make sure the correct data has been downloaded.
    - `Large-Data`: It is recommended to create a folder named Large-Data that will be ignored by GitHub. Save all the source data in this folder after creation.
- Slides
    - `Movie Recommender System.pdf`: Presentation slides to accompany the code including analysis
- `README.md`: This file providing an overview of the project.
- `.gitignore`: .gitignore text file that will ignore a folder named `Large-Data` that you can save your large files to.
