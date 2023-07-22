# Data-Professional-Survey-Visualization

Data Professional Survey Visualization is my first project in Data Analytics. In this project, I did a variety of tasks that you would do on a day-to-day basis such as Data Cleaning, Building Visualizations, and creating a clean dashboard to present the data to extract important information.

# Data Cleaning
Listed here is everything I did concerning cleaning the data
- Empty Columns
    - Cleaned out 5 empty columns.
    - Empty columns serve no purpose as there is no data to extract from them.
    ![ScreenShot](https://github.com/JamesTKapo/Data-Professional-Survey-Visualization/blob/main/Pictures/DeletedEmptyColumns.png?raw=true) 
- Main Column I used to extract data from
    - A column I used a lot was "What title best fits your current role".
    - This column had the depth of our information.
    - This column had an issue with the survey allowing participants to enter "Other" as their occupation and enter in text for what they currently do for work.
    - Created confusing data to look at.
    - Narrowed down the data to just listing occupations as "Other" where this was applicable.
    - Used the Split column function by Delimiter.
        - Created a custom Delimiter to separate the parentheses.
        - This created a new column which I removed as the data didn't become applicable making it completely nullified.
        ![ScreenShot](https://github.com/JamesTKapo/Data-Professional-Survey-Visualization/blob/main/Pictures/Removed%20Column.png?raw=true) 
- Created another Spilt on the “Favorite Programming Language” column
    - Splitting the column with a Delimiter as we had the same issue as previously mentioned.
    - Thereafter I deleted the column for our changed column which again narrowed down the options that were selected from the participants.
- Another column I wanted to use is the "Current yearly salary"
    - This column also needed some adjustments.
    - Firstly I duplicated the column, thereafter I split the column by “Digit to Digit”.
    - There was the string letter “K” used and this was something I deleted as it was completely useless to me.
    - Thereafter I moved over to the second newly created column and removed the string letter K also with the Replace Values function.
    ![Screenshot](https://github.com/JamesTKapo/Data-Professional-Survey-Visualization/blob/main/Pictures/RemovedColumnCurrentYearlySalary_K.png?raw=true)
    - Also removed the symbol - that was found within the column.
    - This created something not only easier to read by also something very easy to work with.
    ![Screenshot](https://github.com/JamesTKapo/Data-Professional-Survey-Visualization/blob/main/Pictures/Replaced%20Values.png?raw=true)
    - Also removed a + within this column and ended up replacing that with the highest salary being 256
    - In the end, I created a custom column that averaged out the salary and to do this I used a DAX function.
    - I split two other columns with Delimiters also such as “What country do you live in” and “Which Industry do you work in” and I had the same issue as previously mentioned with lots of unnecessary characters. After splitting both columns I deleted the ones that were created and narrow down the options.

# Equations I used

***Average Salary***

= ([#"Q3 - Current Yearly Salary (in USD) - Copy.1"] + [#"Q3 - Current Yearly salary (in USD) - Copy.2"]) / 2

![Screenshot](https://github.com/JamesTKapo/Data-Professional-Survey-Visualization/blob/main/Pictures/CustomColumnFormula.png?raw=true)

# Building Out Visualizations

- I created 7 different visualizations to show the data in an easy-to-read format along with something appealing to look at.

***First Visualization***

- Simple Card Visualization displayed the number of participants who took part in the survey, is easy to read, and visualizes the scale at which this survey was taken.

***Second Visualization***

- Simple Card Visualization displayed the average age of participants. Always good to show age or gender demographic and it creates a solid foundation with presenting the other data such as occupation and salary.

***Third Visualization***

- Created a stacked bar chart to show the Average Salary correlated with the Job title. Job title directly impacts the salary you make, making this one of the most important visualizations to have on the dashboard.

***Forth Visualization***

- Wanted to get an idea of what programming language participants used the most in their occupations. As this was a technology-based survey it was important to see what programming language was used most for each position listed in the survey.

***Fifth Visualization***

- The next Visualization I wanted to see was what country these people came from. Although I didn't dive too much into the reasoning for this, county of origin or the country you currently work in has a huge impact on the salary you make and I figured it was important to visualize that. Clicking on the different countries you can see that the values around the dashboard change.
![Screenshot](https://github.com/JamesTKapo/Data-Professional-Survey-Visualization/blob/main/Pictures/ClickingOnTreeMap.png?raw=true)

***Sixths Visualization***

- The next Visualization I used was the gage. I used two gages to display the Happiness of Work-Life Balance and Happiness with Salary.

***Gage one***

- I wanted to Gage how happy people were with their work-life balance, I created min and max values so that we can see the range is between 0 to 10 which is how it showed up on the Survey.

***Gage two***

- I wanted to see how happy people were with their current salary, very important as salary can be one of the contributing factors in how long a person may stay at their job.

***Seventh Visualization***

- The Last Visualization I created was a difficulty chart. I wanted to see how people felt about how difficult it was to break into the field based on several different factors of how they felt such as easy to hard to very difficult.

### Cleaned Everything Up

- Lastly, I did was cleaned everything up on the dashboard so that it was easy to visualize and made everything look appealing as if I were to present the data to other people.
