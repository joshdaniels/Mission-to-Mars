# Mission-to-Mars

## Overview

The mission with this project was to learn web scraping methods to extract information from the NASA Science Mars Exploration website using Chrome Developer tools to identify HTML components, Beautiful Soup/Splinter to automate a web browser and perform the scrape, MongoDB to store the data, and finally Flask to create a web application to display the data. Through the process, the goal was to develop an appt to scrape the following information about the planet Mars:

* Latest News
* Featured Image
* Facts about the planet
* Images of the hemispheres

### Deliverable 1:
To start, we created the file "Mission_to_Mars_Challenge.ipynb" in Jupyter notebook to perform the scraping activity and pull the requested information needed to build the app. Some of the code used include:

Visiting the URL url = 'https://mars.nasa.gov/news/', browser.visit(url)
Using Splinter and BeautifulSoup to automate the browser and parse the HTML element to obtain the latest news title news_soup = soup(html,'html.parser'), slide_elem.find("div",class_='content_title'), news_title = slide_elem.find("div", class_='content_title').get_text()

### Deliverable 2: Update the Web App with Mars’s Hemisphere Images and Titles
Next, we exported our Jupyter notebook file into a Python script. Using this script as the starting point, we started to define the scraping process using Visual Studio Code to edit our Python script. We added functions to scrape through the website(s) and loop through the HTML tags to return the information used to create a database to be stored in MongoDB.

Using the database in Mongo, we create a Flask app to connect to the information and create our app routes. These routes help to display the information on the home page and will perform the scraping of new data using the codes that we wrote in the Python script.

Next, we integrate Mongo into the web app so that the data stored is updated every time the script, "Scraping.py" is run.

After, we create an HTML template to customize the the web app and use Bootstrap components to enhance the HTML and CSS the file.

Lastly, we modified the HTML file to loop through the dictionary and pull the titles and images for the hemispheres of Mars.

### Deliverable 3: Add Bootstrap 3 Components
To complete the final deliverable, the following changes were made to the Bootstrap components to customize the view of the page:

(1) Updated the color of the Jumbotron header by adding gradient color shading and changing the color of the scrape button.
