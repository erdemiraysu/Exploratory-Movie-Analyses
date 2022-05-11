# MOVIE INVESTIGATIONS FOR MICROSOFT
***
## Overview
This project analyzes movie data to provide insights and recommendations about the kind of movies Microsoft should make for their new movie studio.

## Business Problem
***
What type of movies should Microsoft create?

 * Find a way to assess movie “profitability”.
 * Explore characteristics of past movies in relation to profitability: 
     - What genres of movies to make?
     - Which directors to work with?
     - When to release the movie?
     - Which movie length to focus on?

## Data
***
In the folder [zippedData](https://github.com/erdemiraysu/Movies_EDA_Project1/tree/master/zippedData) you will see:

* A dataset from IMDb which involves 4 tables and 140416 Distinct Movies representing movie characteristics such as `genre`, `year`, `runtime`, `director`.
* A dataset from The Numbers which involves `production_budget` as well as `gross` information of 5698 distinct movies

## Methods
*** 
* Derive **profit** (cost minus budget) and **return on investment** (profit/cost times 100) as means to assess "profitability". 
* Use **Median** instead of Mean due to the skewness of the distributions and the presence of outlier movies with extreme success.

## Results and Conclusions
***
WHAT GENRES OF MOVIES TO MAKE?
![Barplot_RoibyBudget_2](https://user-images.githubusercontent.com/61121277/167764190-3d3c98ea-467d-4f43-af94-1fe03a88f232.png)
![Barplot_RoibyBudget_4](https://user-images.githubusercontent.com/61121277/167764199-a1bfa278-e86c-43ba-ad83-46d8816ec952.png)
* With low budget ($4.5-16M), make movies of **Mystery** and **Horror**. They bring more than **300%** ROI and **$25-30M** in profit.
* With high budget (>$40M), make movies of **Animation**, **Adventure** and **Sci-Fi**. They bring close to **200%** ROI but **$200-250 M** in profit.

***
WHEN TO RELEASE THE MOVIE?
![Barplot_ReleaseMonth](https://user-images.githubusercontent.com/61121277/167883905-08beae55-d26d-4bd2-b65f-a32693c1779b.png)
For highest ROI and profit release the movie in **November**. Summer months of **June and July** are also good options. 

***
WHICH DIRECTORS TO WORK WITH?
![Barplot_Directors](https://user-images.githubusercontent.com/61121277/167884337-7af1c31c-3f86-4302-a8ff-86ae26c860b7.png)
For highest ROI and Profit invest on **James Wan, Pierre Coffin, Chris Renaud, Bryan Singer**.

***
HOW LONG SHOULD THE MOVIE BE?
![Barplot_RuntimeMinutes](https://user-images.githubusercontent.com/61121277/167764816-28cd66d8-e0bc-43f1-a5bf-7a8b38f56ce7.png)
For the highest Roi and Profit target **120-140 min** length for the least risk.

## Limitations and Improvements
***
* Small sample size - due to lack of budget and gross information. Perform API calls or wed scraping to increase sample size. 
* Movie names not coded the same way in different datasets - perform a more rigorous cleaning.
* Gather more information about Microsoft’s allocated budget to be able to provide more sensitive suggestions.

***
* The full analysis is in the [jupyter notebook](https://github.com/erdemiraysu/Movies_EDA_Project1/blob/master/MovieProject_Notebook.ipynb). The pdf version of the same notebook is [here](https://github.com/erdemiraysu/Movies_EDA_Project1/blob/master/MovieProject_Notebook.pdf). 
* Summary of the main findings are in the [presentation](https://github.com/erdemiraysu/Movies_EDA_Project1/blob/master/Presentation.pdf). 

## Repository Structure
    .
    ├── images 
    ├── zippedData 
    ├── MovieProject_Notebook.ipynb     
    ├── MovieProject_Notebook.pdf 
    ├── presentation.pdf                                             
    ├── README.md 
    └── movie_data_erd.jpeg   

