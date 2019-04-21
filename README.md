# Using Linear Regression to Predict Video Game Sales

# Project Overview

In this project, I wanted to see if the total sales of a video game can be predicted by knowing general information about the game. As a gamer, I typically have an intuition of how well a game will sell based on my experience following the industry. I wanted to see if I could quantify this intuition into a linear regression model.

<u><b> Key Variables to Predict Sales </b></u>
<br>
* How strongly does the genre of the game affect sales?
* Do certain publishers have a strong record of high sales?
* Is there a certain console which will have a stronger impact on sales than others?
* How much better do franchise games sell than new IPs? 

# Data Collection and Wrangling

I got my data from VGChartz.com as it had all the information I needed as part of my initial hypothesis. If you want to see how I scraped the data from this website, please view my notebook titled: 'Video Game Scraper Notebook'.

Once I obtained the data, I saved it onto a Pandas DataFrame and proceeded to further clean up my data. The Game Title column had contained the information relating to game genre, publisher, and the console, so I parsed through it through a series of lambda functions to create the columns. My Final DataFrame looked like what you see below:

<p align="center">
  <img src="./Images/Final DataFrame.png" title="Data Collected">
</p>

# Exploratory Data Analysis




# Initial Ordinary Least Squares Result

<p align="center">
  <img src="./Images/Initial OLS.png" title="Initial OLS">
</p>

Because most of my data consisted of categorical variables, there isn't a lot I can do to improve this result besides getting rid of the features that had a high P-value since they did not help my model explain the sales of the games. After I got rid of them, my final OLS and coefficients consisted of the following:

<p align="center">
  <img src="./Images/Final OLS.png" title="Final OLS">
</p>

<p align="center">
  <img src="./Images/Final OLS Coefficients.png" title="Final OLS">
</p>
