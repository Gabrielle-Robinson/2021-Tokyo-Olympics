# 2021-Tokyo-Olympics
Quick analysis overview of the 2021 Tokyo Olympics

#About the project
This project is about using data from the 2021 Tokyo Olympics to create barcharts and piecharts that identify particular trends. 
The dataset contains the details of over 11,000 athletes, with 47 disciplines, along with 743 teams taking part in the 2021 Tokyo Olympics. It includes details of the Athletes' name, countries their representing, discipline, gender, and their medals they won, and coaches' name.

Initially I imported the dataset into Google Colab using pyspark and used pandas to create and access the dataframes. Through this I used plotly to create a bar chart representing the number of medals won by each country, deducing that the United States (113), China (88), ROC/Russia (71) and Great Britian (65) and Japan (58) were the top five.

Using pyspark sql I made a SQL query to determine the count of coaches from each country alphabetically, thus generating a data visulization of a heat map. The heat map is relative to the amount of coaches representing each country (Yellow-High to Navy-Low), Japan having the highest amount of coaches following the United States and Spain.

#Download Data
