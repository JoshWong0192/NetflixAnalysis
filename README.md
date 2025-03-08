In this Jupyter Notebook project, I conducted an in-depth analysis of a Netflix dataset, focusing on data cleaning, generate descriptive statistics and create visualisation to uncover key trends and insights.

1. Data Cleaning
- The raw dataset contained various data quality issues, including: null values, redundant values and some duplicated values.

i.Redundant values

![image](https://github.com/user-attachments/assets/56242a93-e13f-4146-97fb-02b25a02c94c)
- The Maturity Rating column contained "U/A" prefixes before age ratings

![image](https://github.com/user-attachments/assets/478e691c-f280-4259-8de8-997ae5bfb460)
- This was cleaned by extracting only the numerical rating (e.g., converting "U/A 16+" to "16+").


