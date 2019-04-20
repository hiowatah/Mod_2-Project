# Using Linear Regression to Predict Video Game Sales

# Project Overview

In this project, I wanted to see if the total sales of a video game can be predicted by knowing general information about the game. As a gamer, I typically have an intuition of how well a game will sell based on my experience following the industry. My intention with this project was to try and quanitify this with a linear regression model.



,
such as the genre of the game, the publisher, the console(s) the game is released on, and finally the average weekly sales. Data was 
collected from VGCharts.com because it contained everything I was looking to obtain. 

If you want to see how I scraped the data from this website, please view my notebook titled: 'Video Game Scraper Notebook'.

Once I obtained the data, I saved it onto a Pandas DataFrame and proceeded to further clean up my data. In order to ensure I was addressing a linear regression problem and not a time series problem, I identified the maximum value of the 'All_Time_Sales' column and identified that as my dependent variable. 

<p align="center">
  <img src="./images/VGChartz.png" title="VGChartz Website">
</p>

