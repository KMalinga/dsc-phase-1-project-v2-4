# Phase 1 Project - Making Microsoft Movie Magic

Within this endeavor, our aim is to thoroughly analyze the multitude of facets crucial for the establishment of a new movie studio. Through the application of coding, mathematical principles, and meticulous data analysis, we will navigate the intricacies of this venture.

* [***Project Overview:***](#project-overview) The project goal, audience, and dataset
* [***Business Problem:***](#business-problem) The client, the endgoal, and the objective
* [***The Data:***](#the-data) The data sets I used
* [***The Process:***](#the-process) Data sorting and cleaning I utilized
* [***Results:***](#results) Data sorting and cleaning I utilized

## Project Overview

In this project, our approach will involve leveraging exploratory data analysis techniques to unearth valuable insights tailored for a business stakeholder envisioning expansion into the realm of movie production. By delving into data-driven exploration, we aim to furnish the stakeholder with a robust plan, empowering them to optimize their investment endeavors effectively.

## Business Problem

Microsoft is poised to venture into the movie-making industry, aiming to make a significant impact. They seek guidance on budgeting, creative direction, and director selection. My task is to analyze the data and provide three strategic business recommendations.
Let's kick things off by tackling these fundamental queries:

### Budgeting and Revenue:
- Determine competitive yet feasible production budgets based on genre and industry benchmarks.
- Utilize predictive modeling to project domestic and global box office revenues.
- Calculate average ROI for target genres and budget ranges.

### Genre and Release Strategy:
- Prioritize genres with proven profitability and align with audience preferences.
- Analyze the impact of parental advisory ratings on audience reach and box office performance.
- Identify optimal release timing based on historical box office data and market trends.

### Runtime Optimization:
- Analyze the correlation between movie runtime and audience engagement.
- Determine the ideal runtime range to maximize viewer retention and theater occupancy.


### For Your Consideration... 
* Are more highly rated movies more profitable?
* What are some highly rated directors in the chosen genre?

## Data Overview

The `Data` folder contains datasets from several sources:

- [IMDB](https://www.imdb.com/): Offers ratings, titles, genres, and director information.
- [Rotten Tomatoes](https://www.rottentomatoes.com/): Provides movie reviews and ratings.
- [TheMovieDB](https://www.themoviedb.org/): Supplies release dates and other details.
- [The Numbers](https://www.the-numbers.com/): Presents insights into production budgets and gross figures.

## Data Processing Approach

Upon reviewing the datasets, specific files and columns were selected for consolidation. The following steps were undertaken:

- Creation of dataframes from SQLite files.
- Standardization of column titles.
- Simplification of date columns to include only the month.
- Conversion of currency strings to float values.
- Resetting of indexes.
- Removal of outliers.
- Normalization of currency values.
- Elimination of redundant columns based on identified issues and trends.


## Results

I focused on scatter plots and bar graphs, labeling each with my recommended budget. Here are some examples:

- **Average Worldwide Gross vs. Production Budget Scatter Plot:**
  ![Average Worldwide Gross vs. Production Budget Scatter Plot](https://github.com/KMalinga/dsc-phase-1-project-v2-4/blob/master/average_worldwide_gross.png)

- **Relationship between Release Months and Average Domestic Gross Bar Graph:**
  ![Relationship between Release Months and Average Domestic Gross Bar Graph](https://github.com/KMalinga/dsc-phase-1-project-v2-4/blob/master/average_domestic_gross.png)

- **Average Rating vs. Domestic Gross Scatter Plot:**
  ![Average Rating vs. Domestic Gross Scatter Plot](https://github.com/KMalinga/dsc-phase-1-project-v2-4/blob/master/avgrat_Domestic_Gross_in_USD_scatter.png)

## Conclusions

- **Budgeting Insights:**
  - Budget around $21 million with an average ROI of $14.5 million. Potential worldwide gross could reach approximately $81 million.
- **Genre, Rating, and Release Timing Recommendations:**
  - Produce an adventure film rated G, with a runtime between 55-65 minutes or 100-145 minutes, and release it in May or June. July and November are backup options.
- **Director Selection Criteria:**
  - Hire a director with international acclaim who has produced highly rated films, like Richard Heap. Higher-rated movies generally yield better box office results globally.

## Next Steps

To further refine our recommendations for Microsoft, future exploration could include:

- **Enhanced Data Analysis:**
  - Utilize more consistent and extensive datasets to gain a deeper understanding, particularly focusing on ratings.
- **Director and Crew Analysis:**
  - Delve deeper into director profiles, considering factors such as prior work experience, film age, and financial success.
- **Marketing Budget Impact Assessment:**
  - Investigate the influence of marketing budgets on ROI, domestic, and foreign gross earnings.
- **Venue Comparison:**
  - Compare various distribution channels (theaters, streaming platforms) to gauge market trends and profitability.

## Non-Technical Presentation

- [Slideshow Presentation](https://github.com/KMalinga/dsc-phase-1-project-v2-4/blob/master/presentation.pdf)

## Repository Structure:

    ├── Data
        └── imdb.db.zip
        └── rt.movie_info.tsv
        └── rt.reviews.tsv
        └── tbdb.movies.csv
        └── tn.movie_budgets.csv

    ├── Images
        └── AWWG_Pro.png
        └── AROI_Pro.png
        └── ARat_Runtime.png
        └── ADGWWG_ParAdv.png
        └── ADG_MR.png
        └── ADG_Gen.png
        └── ADG_ARat.png
     ├── .canvas
     ├── .gitignore
     ├── LICENSE.md
     ├── README.md
     ├── presentation.pdf
     └── student.ipynb
