# -Analysis-of-Lahman-s-Baseball-Player-Data


This report analyzes Lahman’s baseball player database using Python. The analysis involves applying technical documentation, querying SQL data, cleaning and preparing the data, and visualizing it using Python packages. Additionally, three additional questions have been formulated and answered based on the data.
To begin the analysis, extensive technical documentation was researched to understand the structure and content of the SQL database. The documentation provided information on the tables, columns, and their relationships. Understanding the documentation was crucial for formulating appropriate SQL queries and retrieving the desired data for analysis.
The Python package "sqlite3" was utilized to establish a connection to the SQL database file. This package allows executing SQL queries directly within Python. The code executed a query to retrieve data on active players who have played at least 50 games from the "People" and "Batting" tables. The query results were then converted into a Python “pandas” DataFrame for further analysis and manipulation.
After retrieving the data, data cleaning and preparation steps were performed. Missing values were removed from the DataFrame to ensure the quality of the analysis. Calculated columns for player age and full name concatenation were added to provide additional insights. Unnecessary columns related to birth date and name were dropped using “dropna()” function to focus on the relevant variables for analysis.
Python's matplotlib package was used for data visualization. Two types of plots were created: a histogram and a scatter plot. A histogram was created to visualize the distribution of triples per year, providing insights into the frequency of triples over time. A scatter plot was generated to explore the relationship between triples and steals, showcasing the performance of players in terms of both variables.
Data Analysis and Results:
1.	Most Runs Batted In (RBI) from 2015-2018: The code uses SQL to filter the data based on the specified time range and calculates the sum of RBI for each player. 
Output: “Active player with the most RBI from 2015-2018 is arenano01”
2.	Double Plays Grounded Into (GIDP) by Albert Pujols in 2016: The code uses SQL to filter the data to focus on Albert Pujols in the year 2016. 
Output: “Albert Pujols grounded into 24 double plays in 2016.”
3.	Histogram of Triples (3B) per Year: The code creates a histogram using the matplotlib library to visualize the distribution of triples per year. The number of bins is set to 10 for appropriate granularity. Triples are on X-axis and Frequency is on Y-axis.
![image](https://github.com/user-attachments/assets/c84a8078-399a-45a7-9ae3-9539e4d64907)

      
4.	Scatter Plot of Triples (3B) and Steals (SB): A scatter plot was created using the python matplotlib library to examine the relationship between triples and steals. Each data point represents a player's performance in terms of triples and steals. Triples on X-axis and Steals on Y-axis.

![image](https://github.com/user-attachments/assets/c930a647-1ff4-416b-8d1e-4c0e12be0a15)

Additional Questions and Answers:
1.	Question: What is the correlation between batting average (BA) and Home Runs (HR)? 
Answer: By calculating the correlation coefficient between BA and HR, it was found that there is a strong positive correlation between the two variables.
Output: “Correlation between BA and HR: 0.7041675118877206”

2.	Question: Question: Which team had the highest average attendance over the years? 
Answer: the data was grouped by team and the average attendance for each team was calculated using the groupby() function to find the team with the highest average attendance. 
Output: “Team with the highest average attendance: LAN”

3.	Question: What is the correlation between Home Runs (HR) and GIDP? 
Answer: By analyzing the data, it was observed that there is a weak positive relationship between HR and GIDP.
       Output: “Correlation between HR and GIDP: 0.14374276108693368”

In conclusion, this analysis successfully demonstrates the utilization of Python packages to read and apply technical documentation, query SQL data, clean and prepare data, and visualize it. The analysis provided insights into various aspects of baseball player data. Furthermore, three additional questions were formulated and answered, exploring relationships between different variables in the dataset. The project highlights the power of Python for data analysis and lays the groundwork for future improvements and further exploration of the data.
Ideas for Future Improvement: Few things could be explored analyzing the given data; The relationship between player performance and other factors, analyzing trends over different time periods, or building predictive models based on historical data.


