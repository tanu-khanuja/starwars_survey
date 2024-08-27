# Star Wars Movie and Character Analysis

## Overview

This project focuses on data cleaning and analysis using FiveThirtyEight's Star Wars survey data. The primary goal is to clean the dataset for further analysis and to explore insights into movie rankings, view counts, and character familiarity among Star Wars fans.

## Project Structure

- **Data Source**: FiveThirtyEight's Star Wars survey data (`StarWars.csv`)
- **Languages/Tools Used**: Python, Pandas, Plotly

## Files

- `StarWars.csv`: The original dataset used for the analysis.
- `main.ipynb`: The Jupyter Notebook containing the code for data cleaning, analysis, and visualization.
- `README.md`: This file, providing an overview and guide to the project.

## Steps Performed

1. **Data Cleaning**:
   - **Read CSV**: Loaded the CSV file with the appropriate encoding.
   - **Initial Exploration**: Checked the dataset's structure and identified that the 0th row contained column subtitles.
   - **Index Reset**: Dropped the 0th row, reset the index, and renamed columns for clarity.
   - **Mapping**: Mapped `Yes/No` responses to `True/False` and movie names to `True/False`.
   - **Column Type Conversion**: Changed data types for clarity, such as converting `RespondentID` to `int` and ranking columns to `float`.

2. **Data Analysis**:
   - **Average Movie Ranking**:
     - Calculated the average ranking for each Star Wars episode.
     - Visualized the distribution of rankings using a violin plot.
   - **Total View Counts**:
     - Summed up the view counts for each movie episode.
     - Visualized the results using a bar chart.
   - **Gender-wise Analysis**:
     - Analyzed the average rankings and view counts for each episode by gender.
     - Visualized gender-wise distributions using violin plots and bar charts.
   - **Character Familiarity**:
     - Mapped and categorized character familiarity into favorable, neutral, unfavorable, and review unavailable.
     - Visualized character familiarity using a stacked bar chart.

## Key Findings and Visualization

**Movie Rankings**:
  - Episodes II and III are generally favored, with the highest mean rankings.
  - Episode I received consistent rankings but is not the most popular.
  - Episodes V and VI received lower rankings, indicating a divided audience.

<p align="center">
<img src="figures/Distribution of Movie Rankings.png" alt="Distribution of Movie Rankings" width ="700"/>
</p>

Male Respondents:
   - Episodes II and III were rated more favorably by male respondents.
   - Episodes I and IV had more consistent rankings, with less variability in opinions among males.

<p align="center">
<img src="figures/Genderwise Distribution of Movie Rankings - Male.png" alt="Distribution of Movie Rankings" width ="700"/>
</p>

Female Respondents:
   - Female viewers also favored Episodes II and III, but their rankings showed a bit more variability.
   - Episode IV received mixed reactions from female viewers, with a high interquartile range (IQR), indicating either strong approval or disapproval.

<p align="center">
<img src="figures/Genderwise Distribution of Movie Rankings - Female.png" alt="Distribution of Movie Rankings" width ="700"/>
</p>

**View Counts**:
  - Newer episodes have higher view counts, indicating greater popularity or accessibility.
  - Both male and female respondents tend to favor older movies in rankings despite watching newer episodes more.
  
<p align="center">
<img src="figures/Total View Counts of Different Episodes.png" alt="Distribution of Movie Rankings" width ="700"/>
</p>

Genderwise View Counts

- Both male and female respondents watched the newer episodes more frequently than the older ones.
- However, the older movies generally received higher rankings than the newer ones from both genders.
  
<p align="center">
<img src="figures/View Counts of Movies by Gender.png" alt="Distribution of Movie Rankings" width ="700"/>
</p>

- **Character Popularity**:
  - Characters like Han Solo, Luke Skywalker, Princess Leia Organa, and Yoda are widely favored.
  - Characters like Jar Jar Binks and Emperor Palpatine received mixed or unfavorable reviews, reflecting divisive opinions.
 
<p align="center">
<img src="figures/Review of Star Wars Characters Based on Familiarity and Public Sentiment.png" alt="Distribution of Movie Rankings" width ="800"/>
</p>

## How to Use

1. **Clone the Repository**: Clone the repository to your local machine.
2. **Install Dependencies**: Ensure you have Python, Pandas, and Plotly installed. You can use the following command:
   ```bash
   pip install pandas plotly
   ```
3. **Run the Notebook**: Open `main.ipynb` in Jupyter Notebook or Jupyter Lab and run the cells sequentially to perform the analysis.

## Conclusion

This project provides a comprehensive analysis of the Star Wars movies and characters based on survey data. The insights gained can be valuable for understanding audience preferences and character popularity across different demographics. 

Feel free to explore and modify the code to perform further analysis or use the cleaned dataset for other projects.