# Star Wars Movie and Character Analysis

## Project Overview

This project focuses on cleaning and analyzing data from FiveThirtyEight's Star Wars survey. The primary goal is to prepare the dataset for further analysis and extract insights about movie rankings, view counts, and character popularity amongs men and women.

## Project Structure

- **Data Source**: FiveThirtyEight's Star Wars survey data (`StarWars.csv`)
- **Languages/Tools Used**: Python, Pandas, Plotly

## Files

- `StarWars.csv`: The original dataset used for the analysis.
- `main.ipynb`: The Jupyter Notebook containing the code for data cleaning, analysis, and visualization.
- `figures`: This folder contains all the figures generated during the analysis
- `README.md`: This file, providing an overview and guide to the project.

## Steps Performed

1. **Data Cleaning**:
   - **Read CSV**: Loaded the CSV file with the appropriate encoding.
   - **Initial Exploration**: Checked the dataset's structure and identified that the 0th row contained column subtitles.
   - **Index Reset**: Dropped the 0th row, reset the index, and renamed columns for clarity.
   - **Mapping**: Mapped `Yes/No` responses to `True/False` and movie names to `True/False`.

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
   - **Character Popularity by Gender**:
     - Analyzed character popularity separately for male and female respondents.
     - Visualized the data using a stacked bar chart, showing the percentage share of favorable, neutral, and unfavorable responses by gender.

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
<img src="figures/Genderwise Distribution of Movie Rankings - Male.png" alt="Genderwise Distribution of Movie Rankings - Male" width ="700"/>
</p>

Female Respondents:
   - Female viewers also favored Episodes II and III, but their rankings showed a bit more variability.
   - Episode IV received mixed reactions from female viewers, with a high interquartile range (IQR), indicating either strong approval or disapproval.

<p align="center">
<img src="figures/Genderwise Distribution of Movie Rankings - Female.png" alt="Genderwise Distribution of Movie Rankings - Female" width ="700"/>
</p>

**View Counts**:
  - Newer episodes have higher view counts, indicating greater popularity or accessibility.
  - Both male and female respondents tend to favor older movies in rankings despite watching newer episodes more.
  
<p align="center">
<img src="figures/Total View Counts of Different Episodes.png" alt="Total View Counts of Different Episodes" width ="700"/>
</p>

Genderwise View Counts

- Both male and female respondents watched the newer episodes more frequently than the older ones.
- However, the older movies generally received higher rankings than the newer ones from both genders.
  
<p align="center">
<img src="figures/View Counts of Movies by Gender.png" alt="View Counts of Movies by Gender" width ="700"/>
</p>

**Character Popularity**:
  - Characters like Han Solo, Luke Skywalker, Princess Leia Organa, and Yoda are widely favored.
  - Characters like Jar Jar Binks and Emperor Palpatine received mixed or unfavorable reviews, reflecting divisive opinions.
 
<p align="center">
<img src="figures/Review of Star Wars Characters Based on Familiarity and Public Sentiment.png" alt="Review of Star Wars Characters Based on Familiarity and Public Sentiment" width ="800"/>
</p>

Character Popularity by Gender:

 - The analysis shows that male respondents generally have a higher favorable opinion of protagonist characters like Luke Skywalker and Han Solo compared to female respondents.
 - Female respondents showed a more neutral or unfavorable opinion towards antagonist characters like Darth Vader and Emperor Palpatine.

<p align="center">
<img src="figures/Popularity of Star Wars Characters Among Males.png" alt="Popularity of Star Wars Characters Among Males" width ="800"/>
</p>

<p align="center">
<img src="figures/Popularity of Star Wars Characters Among Females.png" alt="Popularity of Star Wars Characters Among Females" width ="800"/>
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

**Note**: This project aims to develop skills in data cleaning and preparation, crucial for effective analysis. However, the dataset used has notable limitations: it may have sampling bias, lacks comprehensive demographic details, and contains inconsistencies such as missing or ambiguous data. These issues mean that the dataset is not fully representative of real-world scenarios, and the results may not accurately reflect broader trends or insights applicable to actual datasets.