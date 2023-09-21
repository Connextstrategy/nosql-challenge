# Python Rutgers Bootcamp Challenge - NOSQL Challenge 

This activity is broken down into three deliverables, Database and Jupyter Notebook Set Up, Update the Database, and Exploratory Analysis

## Description

The UK Food Standards Agency evaluates various establishments across the United Kingdom, and gives them a food hygiene rating. You've been contracted by the editors of a food magazine, Eat Safe, Love, to evaluate some of the ratings data in order to help their journalists and food critics decide where to focus future articles.

## Database and Jupyter Notebook Set Up

1. Import the data provided in the establishments.json file from your Terminal. Name the database uk_food and the collection establishments. Copy the text you used to import your data from your Terminal to a markdown cell in your notebook.

2. Within your notebook, import the libraries you need: PyMongo and Pretty Print (pprint).

3. Create an instance of the Mongo Client.

4. Confirm that you created the database and loaded the data properly:

* List the databases you have in MongoDB. Confirm that uk_food is listed.
* List the collection(s) in the database to ensure that establishments is there.
* Find and display one document in the establishments collection using find_one and display with pprint.

5. Assign the establishments collection to a variable to prepare the collection for use.


## Update the Database

Use NoSQL_setup_starter.ipynb for this section of the challenge.

The magazine editors have some requested modifications for the database before you can perform any queries or analysis for them. Make the following changes to the establishments collection:

1. An exciting new halal restaurant just opened in Greenwich, but hasn't been rated yet. The magazine has asked you to include it in your analysis. Add the following information to the database:

![Screenshot 2023-09-21 114724](https://github.com/Connextstrategy/nosql-challenge/assets/18508699/d2df0c08-320f-4f57-b2cb-0004392c7f19)

2 .Find the BusinessTypeID for "Restaurant/Cafe/Canteen" and return only the BusinessTypeID and BusinessType fields.

3. Update the new restaurant with the BusinessTypeID you found.

4. The magazine is not interested in any establishments in Dover, so check how many documents contain the Dover Local Authority. Then, remove any establishments within the Dover Local Authority from the database, and check the number of documents to ensure they were deleted.

5. Some of the number values are stored as strings, when they should be stored as numbers.

* Use update_many to convert latitude and longitude to decimal numbers.
* Use update_many to convert RatingValue to integer numbers.

## Exploratory Analysis

Exploratory Analysis

### Dependencies


## Import APIs from OpenWeatherMap API & citipy to determine the cities based on latitude and longitude for WeatherPY

* Using Jupyter Notebooks or Visual Studio Code for coding and data visualizations

* *WeatherPY
* import matplotlib.pyplot as plt
* import pandas as pd
* import numpy as np
* import requests
* import time
* from scipy.stats import linregress

## Import APIs from GEOAPIFY for VacationPY
* import hvplot.pandas
* import pandas as pd
* import requests

### Installing

* No modifications needed to be made to files/folders

## Help

The city data that you generate is based on random coordinates and different query times, so your outputs will not be an exact match to the provided starter notebook.

If you'd like a refresher on the geographic coordinate system, this siteLinks to an external site. has great information.

Take some time to study the OpenWeatherMap API. Based on your initial study, you should be able to answer basic questions about the API: Where do you request the API key? Which Weather API in particular will you need? What URL endpoints does it expect? What JSON structure does it respond with? Before you write a line of code, you should have a crystal-clear understanding of your intended outcome.

A starter code for citipy has been provided. However, if you're craving an extra challenge, push yourself to learn how it works by using the citipy Python libraryLinks to an external site.. Before you try to incorporate the library in your analysis, start with simple test cases outside of your main script to confirm that you are using it correctly. Often, when introduced to a new library, learners spend hours trying to figure out errors in their code when a simple test case can save you a lot of time and frustration.

You will need to apply your critical thinking skills to understand how and why we're recommending these tools. What is citipy used for? Why would you use it in conjunction with the OpenWeatherMap API? How would you do so?

While building your script, pay attention to the cities you are using in your query pool. Are you covering the full range of latitudes and longitudes? Or are you choosing 500 cities from one region of the world? Even if you were a geography genius, simply listing 500 cities based on your personal selection would create a biased dataset. Try to think of ways that you can counter these selection issues.

      Hint: Consider the full range of latitudes.

Once you have computed the linear regression for one relationship, you will follow a similar process for all other charts. Optionally, try to create a function that will create these charts based on different parameters. (Note: there will be no extra points for completing this.)

Remember that each coordinate will trigger a separate call to the Google API. If you're creating your own criteria to plan your vacation, try to reduce the results in your DataFrame to 10 or fewer cities.

## Authors

Christopher Manfredi 

## Version History

    * Initial Release

## Acknowledgments

* This is specifically for an exercise for Rutgers Boot Camp 
