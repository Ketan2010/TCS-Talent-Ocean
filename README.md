# TCS-Talent-Ocean Round 2 Submission

**Problem Statement:** Find suitable candidates for project based on required skills and candidates skills <br>

**Approach to solve problem:**  <br>
My approach to solve given problem includes following steps: <br>
1. Get data
2. Data extraction
3. Data cleansing
4. Data manipulation
5. Calculation of matching factor
6. Get suitable candidates on the basis of matching factor

**Algorithm:** <br>
1. Start
2. Create two dataframes for candidate and project details.
3. Extract required columns ( **project id, location, required skills** ) from main dataframe of **project.**
4. **Data extraction:** Extract required columns ( **candidate id, location, skills** ) from main dataframe of **candidate.**
5. **Data manipulation:** Convert both dataframes data into lower case for simplicity of comparison.
6. **Data cleansing:** for both dataframes replace multiples by one.
Example **: java programming, java language, core java, programming in java, java se** can be replaced by simple one-word **java**.
1. Calculate **matching factor** of every candidate for every project
**Matching factor = 90% of (matching skills) + 10% of (location match)**
1. Get top 5 candidates having high matching factor for the project.
2. Final dataframe **(project id, location, required skills, top 5 suitable candidates, matching factor for top 5 candidates.)**

**Requirements:** <br>
Programming language: Python 3 <br>
Python library: Pandas, matplotlib, numpy <br>
Tool used: Google Colab <br>

**Time complexity** : <br>
Time complexity to reach solution using above mentioned approach is:  <br>
T(n) = O(Log( n²)) <br>
