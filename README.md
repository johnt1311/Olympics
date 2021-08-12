# :1st_place_medal: :2nd_place_medal: :3rd_place_medal: Olympics Analysis :1st_place_medal: :2nd_place_medal: :3rd_place_medal:

## Overview
As more than 50,000 athletes, coaches, trainers, and team members head to the land of the rising sun we wondered, "Can Olympic results be predicted?". We analyzed the history of the Summer Olympics to see how past results might help us predict which country will hear their national anthem the most times this year. 

Along with the results of thousands of events our analysis includes non-traditional data including country GDP, country population, life expectancy, and distance from the competing country's capital city to the location of the games. Do these demographic features make a difference in the success of Olympic athletes?

Using advanced machine learning techniques we answer these questions and more on our quest to tackle Tokyo and stand atop the prediction podium. 

### 🎌 From Tokyo to Tokyo 🎌

Japan is one of just six countries who have hosted the Summer Olympics multiple times since 1900. For our analysis we decided to collect data from the first Summer games in Tokyo in 1964, through the most recent Summer games in Rio de Janeiro, Brazil, in 2016. Our data comprised nearly 22,000 medals won by 141 countries in 335 individual and team events.

Our dataset is broken down by competition data and country data. All data points were collected for each year the Summer Olympics were held.

Competition data includes:
* Event 
* Discipline
* Gender
* Competing Country 
* Competition Year
* Host Country
* Winning Countries
* Medal won

Country Data includes:

* GDP
* Population
* Life Expectancy
* Distance from competing country to host country

## The Analysis

Our data provided multiple routes of analysis to determine how economic, demographic, and geographic factors may affect the potential outcomes of Olympic competitions. We analyzed the data with both categorical and projection analyses.

The categorical analysis attempted to classify competing countries into distinct groups. The analysis answered questions such as:

* Do countries with larger populations outperform countries with smaller populations?
* How do medal counts compare when grouping countries by GDP? Is there a connection between GDP and athletic success?
* What if we look at medal count by population and GDP on a per capita basis? Would more countries be qualified as top-tier competitors despite having a lower total medal count?
* Are female competitors from certain countries more successful than male competitors?  

All categorical analysis was performed using a K-Means analysis to determine a number of categories to analyze, and a deep neural network to perform the categorization. 

The projection analysis attempted to estimate the number of medals each country won in the 2021 Olympic games. We analyzed the data using a multi-factor regression model. The multi-factor regression model was then trained and analyzed using a random forest decision tree algorithm. Factors were then analyzed by their importance in the random forest model. 

### Table or visual with the most important factors ###

### Table or visual with the least important factors ###

We determined that binning factors such as.....

We ran the analysis as a boosted model which resulted in....

# The Results
The following results table was created by running our projection model on the 2021 competition data and comparing the results to the actual results of the 2021 games. 

### insert table here ###

Add some insights...


### Other analysis notes ###
Maybe look at how population growth or GDP growth has affected medal counts over the years. 

### Throw in some bar charts or pie charts ###


### Unique aspects of our dataset:

Throughout the years many Olympic athletes have unfortunately been disqualified for various reasons. Disqualified athletes must vacate their medals which are then awarded to the competitor with the next highest finish. Instead of removing the disqualified athletes from our dataset, we chose to view these athletes as their own country, "DQ", to see how they compare to the field.   

During the time period we analyzed countries had been destroyed, created, renamed or merged. We cleaned our dataset to combine countries such as the former USSR and Russia and East Germany and West Germany. These countries are represented by Russia and Germany, respectively, in our dataset.







### Communication protocols:
* Team members communicated through Zoom video calls and Slack messaging
* Code and resources were reviewed by team members through screen sharing and GitHub
* Resources and code were individually committed to team member branches and routinely reviewed and merged to main project branch. 


# Links

Presentation: https://docs.google.com/presentation/d/1THhDSyPohawLwrSiDOjxda2NZSpPXUvQ/edit?usp=sharing&ouid=115662815122483026556&rtpof=true&sd=true
