In this Jupyter Notebook project, I conducted an in-depth analysis of a Netflix dataset, focusing on data cleaning, generate descriptive statistics and create visualisation to uncover key trends and insights.

Data set: NetflixData.csv

Language: Python

Files:
- All in the NetflixAnalysis folder
- The Jupyter Notebook file: NetflixAnalysis.ipynb
- pdf version (For computers that cannot run Jupyter Notebook): NetflixAnalysis_JoshWong.pdf

Tool Used:

Jupyter Notebook → file saved in .ipynb format

Pandas → For displaying the DataFrame.

Matplotlib and seaborn → For plotting different graphs to visualize trends in the dataset.

1. Data Cleaning
- The raw dataset contained various data quality issues, including: null values, redundant values and incorrect format.

(a).Redundant values

![image](https://github.com/user-attachments/assets/56242a93-e13f-4146-97fb-02b25a02c94c)
- The Maturity Rating column contained "U/A" prefixes before age ratings

![image](https://github.com/user-attachments/assets/478e691c-f280-4259-8de8-997ae5bfb460)
- This was cleaned by extracting only the numerical rating (e.g., converting "U/A 16+" to "16+").

(b). Incorrect Format

![image](https://github.com/user-attachments/assets/9c698b10-620f-4bbd-bd3b-7c33d797ee27)
- The Release Year column was originally in decimal format (e.g., 1990.0).

![image](https://github.com/user-attachments/assets/0efa8ba0-f853-445d-97da-a9c1719ce1b7)
- This issue was resolved by converting the data type back to Int64, ensuring accurate representation of years.

(c). Null Values

![image](https://github.com/user-attachments/assets/2ce36546-529c-48a6-9f2f-31f34e06b45c)
- Some columns contain null (missing) values in certain rows, like in Releasing Year and Original Audio

![image](https://github.com/user-attachments/assets/7dcfc0fe-f77b-41e3-a859-b8d12a73fc90)

- To resolve this issue and analyze the movies sorted by year, I used the .notna() function to filter out all rows where the Release Year value is null.

2. Data Visualization
- Created various graphs, including bar charts, pie charts, and line graphs, to visualize trends and analyze the data effectively.

(a). Bar Chart

![image](https://github.com/user-attachments/assets/ae11c96c-7e06-40f2-8ed6-6c305f712563)

- The bar chart displays the top 10 main genres based on the number of movies in each genre, providing insights into the most popular content categories on Netflix.

(b). Pie Chart

![image](https://github.com/user-attachments/assets/4381fccd-3f4a-4d43-ac84-78d2942f2dad)

- The pie chart visualizes the distribution of all main genres, where the top 10 genres are displayed individually, and all remaining genres are grouped into an "Others" category for better clarity.

(c). Stacked Bar Chart

![image](https://github.com/user-attachments/assets/e9c5e003-8ce4-423c-a846-54efe062e69a)

- The stacked bar chart displays the number of movies per main genre for each year from 2010 to 2024, providing insights into genre trends over time. Each bar represents a year, with different colors stacked to show the count of each genre within that year.

(d). Line Graph

![image](https://github.com/user-attachments/assets/7ab483ad-1ae2-42c0-a48b-d60d22363d6e)

- The line graph visualizes the number of Anime movies released each year from 1981 to 2025, showing trends in the popularity of Anime content over time. Each point on the graph represents the count of Anime movies in a given year, helping to identify growth patterns




