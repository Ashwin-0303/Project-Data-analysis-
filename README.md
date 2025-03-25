# Movie Review Analysis - Bookmyshow vs Metacritic Scores

## Project Overview

This project analyzes movie review scores from three popular sources: Bookmyshow, Metacritic, and IMDB. By comparing Bookmyshow scores with Metacritic ratings, we attempt to investigate the possible differences in the way these platforms rate movies and whether there's a correlation between the two. Linear regression is used to model the relationship between Bookmyshow and Metacritic scores, and various visualizations (e.g., histograms, scatter plots) are generated to support the analysis.

## Dataset

The dataset used in this project is the `Bookmyshow_score_comparison.csv`, which includes movie review scores from multiple sources, including Bookmyshow and Metacritic. The dataset contains the following columns:

- **Bookmyshow_Stars**: Movie ratings from Bookmyshow.
- **Metacritic_norm_round**: Normalized Metacritic ratings rounded to the nearest integer.
- **IMDB**: IMDB ratings for movies.
- Other relevant columns like movie titles and other review sources.

## Tools Used

- **Pandas**: For data manipulation and analysis.
- **Matplotlib**: For visualizing data with plots.
- **NumPy**: For numerical operations.
- **SciPy**: For performing linear regression and statistical analysis.
- **Seaborn**: For creating visually appealing and informative statistical plots.
  
## Steps Taken

1. **Data Loading and Inspection**:
   - Loaded the dataset into a Pandas DataFrame and examined the first few rows to understand its structure.

2. **Exploratory Data Analysis**:
   - Created histograms to compare the distributions of Bookmyshow and Metacritic scores.
   - Observed that Bookmyshow scores are generally higher than Metacritic ratings, with a noticeable absence of scores lower than 3 on Bookmyshow.

3. **Descriptive Statistics**:
   - Calculated the mean and median values for both Bookmyshow and Metacritic scores.
   
4. **Correlation Analysis**:
   - Performed a scatter plot to visually assess the correlation between Bookmyshow and Metacritic scores.
   - The correlation appeared low, meaning that Bookmyshow and Metacritic scores are not highly related.

5. **Linear Regression**:
   - Performed linear regression to quantify the relationship between Metacritic and Bookmyshow scores.
   - Used the regression equation to predict Bookmyshow scores for Metacritic scores of 1, 3, and 5.

6. **Visualization**:
   - Generated various visualizations, including scatter plots and histograms, to illustrate the analysis.

## Results

- **Descriptive Statistics**:
  - The mean Bookmyshow score is **4.09** and the median is **4.0**.
  - The mean Metacritic score is **2.97** and the median is **3.0**.
  - The analysis showed that Bookmyshow generally gives more favorable reviews than Metacritic.

- **Correlation**:
  - A scatter plot and linear regression analysis showed a **low correlation** between the Metacritic and Bookmyshow scores. This suggests that the scores from these two sources are not strongly related.

- **Linear Regression**:
  - The regression model predicts that for a Metacritic score of 3, the Bookmyshow score is approximately **4.09**.
  - The equation of the regression line is:  
    \( Bookmyshow\_Stars = 0.097 \times Metacritic\_norm\_round + 3.80 \)
