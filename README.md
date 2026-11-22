# SpaceX Falcon 9 Landing Prediction

This is my final project for the IBM Data Science Professional Certificate.

I worked with SpaceX Falcon 9 launch data. I wanted to see which factors are related to successful first-stage landings. I also tested if machine learning models could predict the landing outcome.

## What I did

This was a guided IBM project. The labs included instructions and starter code. I completed the assigned tasks, ran the notebooks and checked the results. I did not write the whole project from scratch.

- I tried to collect data from the SpaceX REST API.
- I used requests and BeautifulSoup to get Falcon 9 launch data from Wikipedia.
- I cleaned the data with Pandas and created a column for landing success.
- I used SQL to check launch sites, payload mass and mission outcomes.
- I made charts with Matplotlib and Seaborn.
- I used Folium to show launch sites and nearby locations on maps.
- I built a Plotly Dash dashboard with a dropdown menu and a payload slider.
- I trained four classification models: Logistic Regression, SVM, Decision Tree and KNN.

## Results

The landing success rate generally increased over the years. The results also changed across launch sites and orbit types.

I used GridSearchCV to test different model settings. I had to correct an unsupported parameter in the Decision Tree model and train it again.

The final test accuracy was:

| Model | Test accuracy |
| --- | --- |
| Logistic Regression | 83.33% |
| SVM | 83.33% |
| Decision Tree | 88.89% |
| KNN | 83.33% |

Decision Tree had the highest test accuracy. It made 16 correct predictions out of 18. It predicted 12 successful landings and 4 failed landings correctly. It predicted 2 failed landings as successful.

## API issue

Some SpaceX API requests failed during the data collection lab. I got a JSONDecodeError and could not finish that part. I continued the other labs using the datasets provided by IBM.

## Project files

The repository contains my Jupyter notebooks for data collection, data wrangling, SQL, visualizations, Folium and machine learning. It also contains the Python file for the Plotly Dash app.

## Tools

Python, Pandas, SQL, Matplotlib, Seaborn, BeautifulSoup, Folium, Plotly Dash and scikit-learn.
