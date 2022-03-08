# 2021-Tokyo-Olympics
Quick analysis of the 2021 Tokyo Olympics

# About the project
This project is about using data from the 2021 Tokyo Olympics to create barcharts and piecharts that identify particular trends. 
The dataset contains the details of over 11,000 athletes, with 47 disciplines, along with 743 teams taking part in the 2021 Tokyo Olympics. It includes details of the Athletes' name, countries their representing, discipline, gender, and their medals they won, and coaches' name.

Initially I imported the dataset into Google Colab using pyspark and used pandas to create and access the dataframes. Through this I used plotly to create a bar chart representing the number of medals won by each country, deducing that the United States (113), China (88), ROC/Russia (71) and Great Britian (65) and Japan (58) were the top five.

Using pyspark sql I made a SQL query to determine the count of coaches from each country alphabetically, thus generating a data visulization of a heat map. The heat map is relative to the amount of coaches representing each country (Yellow-High to Navy-Low). Is is noted that Japan (35) had the highest amount of coaches at the Olympics following the United States (28) and Spain (28). The countries that had the lowest amount of coaches at the Olympics were Angola, Bahrain, Belarus, Cambodia, Croatia, Honduras, Liechtenstein, Portual, Slovakia, Tunisia, and Turkey who all had only 1.

Using pyspark sql once again I gathered the count of athletes in each country representing each discipline at the Olypmics. With this information I created a bar char of the altletes from each country per discipline, deducing that the top five discplines at the Olympics were Athletics (2068), Swimming (743), Football (567), Rowing (496), and Hockey (406). I once again created a bar char of the number of athletes splits by the top thress disciplines.

The last data visualization made was multiple subplots representing the percentages of males and females in each discipline. This was accomplished by specifying the organizational  layout of the pie charts and then specifying the number of columns and rows for each pie chart. Then I created a loop that added a subplot after another subplot by using the iterrow function. From there I used pandas to identify the differents teams representing a country and which event the teans was in.

# Download Data
To download data, copy this repo using git clone https://github.com/Gabrielle-Robinson/2021-Tokyo-Olympics, open the file '2021-olympics-in-tokyo.zip', then download and unzip file. 

# How to Run
Open file '2021_Tokyo_Olympics.ipynb', click 'Open in Colab', and then run code.
