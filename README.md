# Movie Review Analysis - Bookmyshow vs Metacritic Scores

## Project Overview
This project analyzes movie review scores from three popular sources: **Bookmyshow**, **Metacritic**, and **IMDB**. By comparing **Bookmyshow** scores with **Metacritic** ratings, we investigate the possible differences in the way these platforms rate movies and explore whether there's a correlation between the two. 

**Linear regression** is used to model the relationship between Bookmyshow and Metacritic scores. Additionally, various **data visualizations** (e.g., histograms, scatter plots) are generated to support the analysis. 

In this project, **Python** was used for data manipulation, statistical analysis, and linear regression, while **Tableau** was used to create interactive and visually compelling visualizations of the data.

## Dataset
The dataset used in this project is the **Bookmyshow_score_comparison.csv**, which includes movie review scores from multiple sources, including Bookmyshow and Metacritic. The dataset contains the following columns:

- **Bookmyshow_Stars**: Movie ratings from Bookmyshow.
- **Metacritic_norm_round**: Normalized Metacritic ratings rounded to the nearest integer.
- **IMDB**: IMDB ratings for movies.
- **FILM**: The name of the movie (for identification).
- **Other relevant columns**: Other review sources.

## Tools Used
- **Pandas**: For data manipulation and analysis.
- **Matplotlib**: For visualizing data with plots.
- **NumPy**: For numerical operations.
- **SciPy**: For performing linear regression and statistical analysis.
- **Seaborn**: For creating visually appealing and informative statistical plots.
- **Tableau**: For interactive data visualization and dashboard creation.

## Steps Taken

### 1. Data Loading and Inspection
- Loaded the dataset into a **Pandas DataFrame** and examined the first few rows to understand its structure and clean the data for analysis.

### 2. Exploratory Data Analysis
- **Python Visualization**: Created histograms to compare the distributions of **Bookmyshow** and **Metacritic** scores using **Matplotlib**.
    - Found that **Bookmyshow scores** tend to be higher than **Metacritic scores**, with a noticeable absence of scores below 3.
  
- **Tableau Visualization**: In Tableau, histograms were created for both **Bookmyshow** and **Metacritic** scores. The visualizations provided an interactive platform to explore the distributions and gain deeper insights into the rating patterns. Users could filter by specific films to see score distributions for individual movies.

### 3. Descriptive Statistics
- **Python Analysis**:
    - The mean and median values for both Bookmyshow and Metacritic scores were calculated:
        - **Bookmyshow mean**: 4.09, **Bookmyshow median**: 4.0
        - **Metacritic mean**: 2.97, **Metacritic median**: 3.0
    - These statistics indicated that **Bookmyshow** tends to give higher ratings than **Metacritic**.
  
- **Tableau Insights**: In Tableau, **calculated fields** were used to compute the mean and median values dynamically. These statistics were displayed on the dashboard to highlight the central tendency of each source's ratings.

### 4. Correlation Analysis
- **Python Analysis**:
    - A **scatter plot** was created to visually assess the relationship between **Bookmyshow** and **Metacritic** scores.
    - The correlation appeared low, suggesting that there was not a strong linear relationship between the two.
  
- **Tableau Analysis**: 
    - A **scatter plot** was created in Tableau to visualize the relationship between **Bookmyshow** and **Metacritic** scores.
    - Users could interact with the plot, zoom in/out, and filter based on movie titles to explore individual data points.
    - Tableau's **Trend Line** feature was used to visualize any linear relationship, showing that the correlation between the two platforms' scores was indeed low.

### 5. Linear Regression
- **Python Analysis**:
    - Linear regression was performed to quantify the relationship between **Bookmyshow** and **Metacritic** scores.
    - The regression equation was: 
        \[
        \text{Bookmyshow\_Stars} = 0.097 \times \text{Metacritic\_norm\_round} + 3.80
        \]
    - Predictions for Bookmyshow scores were made for Metacritic scores of 1, 3, and 5.
  
- **Tableau Regression**: 
    - In Tableau, the **linear regression line** was overlaid on the scatter plot to further illustrate the relationship.
    - The regression equation was displayed dynamically within the visualization, and users could filter or adjust the view to see how the relationship varies for different subsets of movies.

### 6. Visualization
- **Python Visualization**:
    - Generated various visualizations, including **scatter plots** and **histograms**, to illustrate the distribution of ratings and the correlation between the scores.
    - The **fm_diff** column was calculated to measure the absolute difference between Bookmyshow and Metacritic scores, highlighting the largest discrepancies.
  
- **Tableau Visualizations**:
    - **Histograms** for both **Bookmyshow** and **Metacritic** scores were created to provide insights into their distributions.
    - A **scatter plot** showed the relationship between **Bookmyshow_Stars** and **Metacritic_norm_round**. The regression line was added to this plot for a clearer understanding of the relationship.
    - An interactive **dashboard** was created, incorporating the scatter plot, histograms, and summary statistics for **Bookmyshow** and **Metacritic** scores, providing users with a dynamic way to explore the data.
    - **Calculated fields** like the **fm_diff** were used to create visual representations of the discrepancies between the two ratings, sorted by the largest differences.

## Results

### Descriptive Statistics:
- **Bookmyshow mean**: 4.09, **Bookmyshow median**: 4.0
- **Metacritic mean**: 2.97, **Metacritic median**: 3.0
- **Observation**: Bookmyshow generally gives more favorable reviews than Metacritic.

### Correlation:
- A **scatter plot** and **linear regression** analysis showed a low correlation between **Metacritic** and **Bookmyshow** scores, indicating that the ratings from these two sources are not strongly related.

### Linear Regression:
- The regression model predicts that for a **Metacritic score of 3**, the **Bookmyshow score** would be approximately **4.09**.
- The equation of the regression line is:
  \[
  \text{Bookmyshow\_Stars} = 0.097 \times \text{Metacritic\_norm\_round} + 3.80
  \]

### Tableau Insights:
- Interactive dashboards in Tableau helped visualize the **distribution** and **relationship** between the ratings from different sources.
- Users could explore the data interactively, drill down to specific films, and visualize the regression model dynamically. The visualizations provided additional context by allowing comparisons between **Bookmyshow**, **Metacritic**, and **IMDB** scores for each movie.

## Conclusion
- This project provided an in-depth analysis of movie review scores from **Bookmyshow** and **Metacritic**, with **Python** used for statistical analysis and **Tableau** used for interactive visualizations.
- The comparison between the two platforms revealed **significant differences** in their rating tendencies, and the **low correlation** between Bookmyshow and Metacritic suggests that the two platforms have different review processes and scoring criteria.
- The **linear regression model** provided a mathematical framework to predict **Bookmyshow** ratings based on **Metacritic** scores, but the **low correlation** indicated that predictions may not be highly accurate for all movies.

---

This README provides a complete overview of the project, including how the analysis was done using **Python** for data manipulation and **Tableau** for visualizations. Feel free to modify it based on your project specifics or repository structure.
