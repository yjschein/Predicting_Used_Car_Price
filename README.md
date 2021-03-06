# Predicting the Price of a Used Car

## Purpose of the project: 

In this project, I created a model to predict the price of used cars based on a used cars dataset from Kaggle. I created graphs using Pandas and Seaborn to help visualize the data. The graphs were also useful in identifying the most important features in the data set. Some of the charts emphasize the most effective features while others such as mileage and age of car while other assist in visualizing the statistical testing. The features which are seen in the graphs all helped build my model and helped visualize the results. After the data was uploaded, I cleaned and organized the data so that it is useful for other people to analyze and draw their own conclusions. Below I will share a few of my graphs and then explain my final model. 

## Data Source
The dataset that I used for this project was webscraped from craigslist and downloaded from Kaggle. It originally had 435,849 rows, but was shrunken down in the data cleaning phase. Some of the features included the year, manufacturer, model, odometer as well as 21 other features. 

## Data Cleaning
The data cleaning phase was a lot of work due to the high number of missing and strange values. This often occurs on websites where anyone can edit and post anything. In this case it was very messy because anyone can go on craigslist and post their car and often there were absurd prices in the millions of dollars for cars that would normally only be worth a couple thousand dollars. The following features were ones that I dropped because they did not offer valuable information: url, region_url, title_status, vin = drop, size, paint_color, image_url, description, county, lat, long. Some of the important features included in this project were model, condition, manufacturer, year etc. 

## Graphs:
1. I graphed the fuel type against the average price for each fuel type to see which type of used car costs the most. I found that electric cars cost on average $10,000 more than gas cars. This is not surprising due to the innovation and excitement that comes along with purchasing an electric car. Furthermore, as a result of purchasing an electric car, the owner is saving thousands of dollars in gas, as well as, time because he or she no longer needs to go to the gas station to fill up his or her car. 
![fuelPrice](images/Fuel_vs_Price.png)
2. I graphed the total miles used by the car (odometer) against the price of the car to see what the effect is. I found that the more miles a car accumulated costs more than a car with fewer  miles 
![odometerPrice](images/Odometer_vs_Price.png)
3. Lastly, I plotted the age of the car against the average price of the car for that model year. As you can see, there is an inverted bell curve describing the price of cars against the year. As a car approaches the early 2000’s the car is relatively cheap, as opposed to a newer car closer to 2020 or a car that is antique from the mid 1900’s. 
![yearPrice](images/Year_vs_Price.png)

## Model: 
In my model, I included 15 features excluding the dummy columns. For example, I included the condition of a car, manufacturer, state that the used car is being sold in and many more features to help my model. I started off with a baseline model and used RMSE as my evaluation metric due to the fact that it penalizes larger errors. Originally my model was off by an average of $9722.34 per car. Eventually, after testing out different machine learning metrics, my model was only off by a little over $7,000. 

## Next Steps
The model performed well, but in the future I would like to improve it. For example, I would like to break up the states feature into fewer categories. 

## Conclusion: 
In conclusion, my model was about $7000 off from predicting the true price of a car.
