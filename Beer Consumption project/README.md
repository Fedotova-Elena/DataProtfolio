# Beer consumption in São Paulo.

[data sourse](https://www.kaggle.com/dongeorge/beer-consumption-sao-paulo/code)
[Jupiter Notbook](https://github.com/Fedotova-Elena/DataProtfolio/blob/main/Beer%20Consumption%20project/beer%20consumption_final.ipynb)
## Introduction

The data (sample) was collected in São Paulo — Brazil, in a university area, where there are some parties with groups of students from 18 to 28 years of age (average).

What can influence consumer's decision to grab a beer? Could it be bad weather, season or something else? 
In this project I tried to answer this question. 

**Buisness problem**

Keeping the right amount of product in stock is critical to businesses. Having too little means running out at inopportune times, causing customers to buy elsewhere. Having too much means paying unnecessarily high costs for storage and inventory management. This project can help to improve supply chain managment and forecast seasanal level of consumption. 

### Technology 

Data Cleaning, data exploration and modeling was all done in **Python** using the **Jupyter Notebook**.

### Research Questions:
- Will beer consumption vary when there is change in weather conditions?

- Do weekends and weekdays play their role in beer consumption?

- Which season and month of the year have more beer consumption?

### Goal of This Project

Build a linear regression to predict how much beer will be consumed. 

## Data Analysis 

###  Data cleaning process

-	translated the columns name from Portuguese to English
-	checked and changed columns type where it was needed
-	I found empty rows below the rows with data that I could safely drop

Also, for better understanding the data I decided to declare the weather seasons.  Brazil lies in the Southern Hemisphere, Spring is October through November, Summer is December through March.

### EDA 

First, I did a heatmap of the Variables to see what influences beer Consumption.
-	Maximum Temperature(0.64)
-	Median Temperature(0.57)
-	Weekend(0.51)
[heatmap](heatmap.png)

Now I’ll explore the weather (Temperature and Precipitation) in São Paulo throughout the year. In São Paulo, the summers are warm, muggy, wet, and mostly cloudy and the winters are short, cool, and relatively dry.

[Temperature Over the Year in São Paulo](annual_temp.png)
[Precipitation Over the Year](annual_rain.png)

In autumn less beer were consumed than in other seasons.

[Average Beer Consumption by Season](beer_consumption_season.png)
[Summer](Summer.png)
[Autumn](Autumn.png)
[Winter](Winter.png)
[Spring](Spring.png)

On the charts we see strong correlation between temperature and beer consumption, precipitation and beer consumption.
People drink more when the weather is dry and warm. Also, the highier the temperature, the more liters of beer were consumed. 

[Beer Consumption Temperature and Precipitation](beer_consumption_temp_rain.png)

People consume more beer on weekends than on weekdays. No surprise here!

[Beer Consumption Over the Week](beer_consumption_weekday.png)

## Modeling

Simple linear regression is commonly used in forecasting.
I built a Linear Regression Model with accuracy score 72% to predict beer consumption based on the weather temperature throughout the year and day of the week.

## Recomendation 

Before using this model for adjusting and modifying the supply chain I would suggest to find and add more relative data to this data set to make the prediction more accurate. 
The list of the official holidays in Brazil, soccer/football games schedule would be useful and since this data is relative to the university area, it would be great to know important days from a student schedule, for example, when they got breaks.

