# PythonWeatherApp
Final project for my intro to Python course is a interactive Weather App using Python that pulls real time data from an API.

## Installation:
-Using the latest version of PyCharm CE you will need to import requests

-Obtain an API key from OpenWeatherMap to access the information

-Use the following link to obtain the url data to incorporate into your code 'https://openweathermap.org/api'

-This specfic program utilizes the 'Current Weather Data' API document


## Loading Data:
-Assign the beginning url and api key to two separate variables 

-Example:
      zip_url = "https://api.openweathermap.org/data/2.5/weather?q="
          key_api = 'c8541d95699838c63c2443eca4e5dae9'

## Code:
-Create two functions one for looking up the weather by zip code and the other looking up the weather by city and state

-Both of these functions will be relatively the same aside from the zip and city specific code

-This code is built within a try and except function to exit the program if the zip code or city was not found

-The first try and except function asks the user for input on the zip code they want to check the weather for, if the zip code exists in the api then if will move on to the next try and except function. If the zip code doesn't exist the program will exit.

-Print statements are added to provide context to the user on how to fix the issue

-Example:
          try:
              postal = int(input('Type in your zip code: '))
          except ValueError:
              print('You need to enter a numerical value.')
              print('Program exited.')
              exit()

-The next try and except function plugs the user's zip code into the url to complete the the url

-

