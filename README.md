# Movie Recommender System

## Overview
This project aims to analyze movie review data with the end goal being to create a recommender system that can recommend movies based on movie ratings from other users that like similar movies to the ones searched in the recommender system. By following the steps in this project, you can create a recommender system that will allow you to search a movie and be given  new movies to watch based on their similarity to the movie searched.

## Problem Statement
I have been tasked by a start-up company that aims to help movie lovers find new content. They are building an application that will store users movie watching history and their ratings of the movies they have watched. They have tasked me with finding a way to use the data they will have from their users to help recommend them new content.<br> 

Since the founders connected over their love of movies, it is important to them that these recommendations fit the interests of their users, so I will be building them a recommender system that can take the movie ratings from users and find other movies that people with similar interests rated highly. Another point of interest will be how to manage the data that they have on movie ratings to see what should be included in a recommender system.

## Analysis
In my findings, there were a few things that were very clear. First, the amount of data that is included in the model greatly increased its performance. Having a large pool of user reviews allowed the model to find similar movies more effectively. This did make it harder to set up the recommender system, since increasing the users and movies that were included increased the size of the matrix that the recommender system is built on. A balance of data needed to be selected where accurate recommendations were given without maxing out the computing power. In practice, this can be solved with cloud computing.

That being said, performance also increased when putting a minimum on the number of reviews a user has made. This is because users with a smaller number of reviews had a smaller opportunity for the model to find similarites in the movies they did review. A minimum number of reviews for a specific movie also increased the performance for similar reasons.

## Recommendations
My first recommendation is for the start-up to begin collecting user rating data immediately so that they can build up the history of ratings in their database. Since the number of users and reviews improved the recommender system.

The second is to build an application that can use the recommender system that was made in this project to recommend movies to customers who are not users with the data they have on their customers. This can help draw in new users for the company, which in turn will increase the number of users and reviews they can add to their recommender system data.

Thirdly, I recommend using a cloud service like AWS for computing. Computing power was a major issue in this project, so if they want a high functioning recommender, they will need to invest in computing power to make sure its performance is top tier.

Lastly, place a minimum threshold on the users and movies that are included in the recommender system. Users that have a low number of reviews will still be able to get recommendations, but they must have a history of reviews before their ratings are included. This will ensure the quality of the recommendations.

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
