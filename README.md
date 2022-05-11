# MOVIE INVESTIGATIONS FOR MICROSOFT
***
## Overview
This project analyzes movie data to provide insights and recommendations about the kind of movies Microsoft should make for their new movie studio.

## Business Problem
***
What type of movies should Microsoft create?

 Find a way to assess movie “profitability”.
 Explore characteristics of past movies in relation to profitability: 
 * What genres of movies to make?
 * Which directors to work with?
 * When to release the movie?
 * Which movie length to focus on?

## Data
***
In the folder zippedData you will see:
* A dataset from IMDb which involves 4 tables and 140416 Distinct Movies representing movie characteristics such as `genre`, `year`, `runtime`, `director`.
* A dataset from The Numbers which involves `production_budget` as well as `gross` information of 5698 distinct movies

## Methods
*** 
* Derive **profit** (cost minus budget) and **return on investment** (profit/cost times 100) as means to assess "profitability". 
* Use **Median** instead of Mean due to the skewness of the distributions towards right and the presence of outlier movies with extreme success.

## Results
***
![Barplot_RoibyBudget_2](https://user-images.githubusercontent.com/61121277/167764190-3d3c98ea-467d-4f43-af94-1fe03a88f232.png)
![Barplot_RoibyBudget_4](https://user-images.githubusercontent.com/61121277/167764199-a1bfa278-e86c-43ba-ad83-46d8816ec952.png)
