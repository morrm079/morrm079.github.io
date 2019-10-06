---
layout: post
title:      "King County Data Science Project"
date:       2019-10-06 20:19:21 +0000
permalink:  king_county_data_science_project
---


What a great feeling it is to have completed my first data science project. I have to admit at first, it was quite overwhelming, but as I worked through the data, I became more confident in what I was doing. It was a great learning experience, that is for sure. First, let me give you some background about the project.

We were given a data set of sale prices of homes in King County. Along with the sale prices, other features were given such as square footage of the home and the number of bedrooms and bathrooms in each house. With this data, we were asked to predict the sale prices of other houses.

I knew the first step I needed to take was to clean my data, I dove right in. That was my first mistake, diving right in without a plan. Instead, I should have created an outline of what action I planned on taking. As I went through my project, I found myself going back and adding and deleting info. Which at first didn't seem like a big deal, but caused issues down the line because I wasn't updating lines of code below my new additions. And I didn't notice the impact this had until a bit later into my project when I was checking for multicollinearity.

It was quite frustrating when I couldn't understand why the code I was using to remove a feature wasn't working. With some advice, I was able to figure out where I went wrong and fix the issue. It was time consuming, but a good learning process, one I hope not to repeat on future projects. 

After I checked for multicollinearity, I began checking my data for outliers. This was pretty straightfoward. It helped having a sense of what the average home was like, so seeing a house listed with 33 bedrooms was a good indicator that I needed to remove some of these out of the ordinary homes from the data set, otherwise it might skew my results. To help removed outliers, I used box plots. By plotting the data with box plots, I was able to recognize what features need to be worked on and how to update the data.

Then I was able to do some feature creation! To learn a little more about my data set, I created a feature called price_per_sqft (price per square foot). With this info, we could learn more info about a certain area. I figure the higher the price per square foot, the more desirable the neighbor. Location, location, location! This was also helped to create my model.

Then I used OLS regression to run stats on my inital set of featured variables. After that, I used feature ranking with recursive feature elimination to rank which on the feature variables were most important. I then took the 9 highest rated features and re-ran the OLS regression. I was able to obtain a 0.914 R squared value with the 9 highest rated features.


