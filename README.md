# SpaceX Falcon 9 Landing Prediction

This is my final project for the IBM Data Science Professional Certificate.

I worked with SpaceX Falcon 9 launch data. I wanted to see which factors are related to successful first-stage landings. I also tested if machine learning models could predict the landing outcome.

## What I did

This was a guided IBM project. The labs included instructions and starter code. I completed the assigned tasks, ran the notebooks and checked the results. I did not write the whole project from scratch.

Data collection: I worked on the SpaceX API requests, but some calls failed. In the web scraping lab, I extracted launch records from Wikipedia tables and saved them in a Pandas DataFrame.

Data wrangling: I checked missing values, counted landing outcomes and created the Class column (1 for a successful landing, 0 otherwise).

Data visualization: I completed scatter plots, a bar chart and a line chart. I compared flight number, payload mass, launch site, orbit type and landing success over time.

SQL: I wrote queries to find launch sites, filter records, calculate payload statistics and count different mission and landing outcomes.

Folium: I added launch site markers and colored landing outcome markers. I also measured distances to nearby points, including a railway, a highway and the coastline.

Plotly Dash: I completed the dropdown, payload range slider and callback tasks in the provided dashboard app. I used a pie chart and a scatter plot to explore the results.

Machine learning: I completed the preprocessing and classification tasks with Logistic Regression, SVM, Decision Tree and KNN. I used GridSearchCV to compare parameter settings and checked accuracy scores and confusion matrices.

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
