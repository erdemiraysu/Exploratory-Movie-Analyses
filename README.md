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
In the folder zippedData you will see:
* A dataset from IMDb which involves 4 tables and 140416 Distinct Movies representing movie characteristics such as `genre`, `year`, `runtime`, `director`.
* A dataset from The Numbers which involves `production_budget` as well as `gross` information of 5698 distinct movies

## Methods
*** 
* Derive **profit** (cost minus budget) and **return on investment** (profit/cost times 100) as means to assess "profitability". 
* Use **Median** instead of Mean due to the skewness of the distributions and the presence of outlier movies with extreme success.

## Results and Conclusions
***
WHAT GENRES OF MOVIES TO MAKE?
* With low-medium budget ($4.5-16M), make movies of Mystery and Horror. They bring more than 300% ROI but about $25-30M in profit.
* With high budget (>$40M), make movies of Animation, Adventure and Sci-Fi. They bring close to 200% ROI but close to $200-250 M in profit.
![Barplot_RoibyBudget_2](https://user-images.githubusercontent.com/61121277/167764190-3d3c98ea-467d-4f43-af94-1fe03a88f232.png)
![Barplot_RoibyBudget_4](https://user-images.githubusercontent.com/61121277/167764199-a1bfa278-e86c-43ba-ad83-46d8816ec952.png)

***
WHEN TO RELEASE THE MOVIE?
For high ROI and profit release the movie in **November**. Summer months of **June and July** are also good options. 
![Barplot_ReleaseMonth](https://user-images.githubusercontent.com/61121277/167764690-988e8c47-3b7d-4a12-bc6e-35667db1f45c.png)

***
WHICH DIRECTORS TO WORK WITH?
![Barplot_Directors](https://user-images.githubusercontent.com/61121277/167765019-64ce3377-c119-4c17-bd20-3f89ff915853.png)
For smaller budget movies where we care more about ROI invest on **Chris Lofing** and **Travis Cluff**
For bigger budget movies where we care more about PROFIT invest on **Atsushi Wada** and **Kevin Lincoln** 

***
HOW LONG SHOULD THE MOVIE BE?
For the highest Roi and Profit target **120-140 min** length for the least risk.
![Barplot_RuntimeMinutes](https://user-images.githubusercontent.com/61121277/167764816-28cd66d8-e0bc-43f1-a5bf-7a8b38f56ce7.png)

## Limitations and Improvements
***
* Small sample size - due to lack of budget and gross information. Perform API calls or wed scraping to increase sample size. 
* Movie names not coded the same way in different datasets - perform a more rigorous cleaning.
* Gather more information about Microsoft’s allocated budget to be able to provide more sensitive suggestions.

***
* The full analysis in the Jupyter Notebook - MovieProject_Notebook.ipynb. 
* Summary of the findings are in the presentation.pdf. 

## Repository Structure
    .
    ├── zippedData
    ├── MovieProject_Notebook.ipynb                        
    ├── README.md                    
    ├── movie_data_erd.jpeg                 
    ├── presentation.pdf                
    ├── gitbhub.pdf
    └── MovieProject_Notebook.pdf

