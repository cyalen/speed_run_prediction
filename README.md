# Classification using Ensemble Methods: Predicitng World Record Speedruns of Super Mario 64

This project, which I completed as part of my individual courswork for my Predictive Analytics module at UCL, takes run data from the Speedrun.com API and uses it to train a model to predict which runs are classified as "WR  runs" across the main speedrunning leadeboards for Super Mario 64.

This project was conceived with the intent to serve as a baseline for solving discoverability problems for speedrunners on Twitch and Youtube, as hyper-popular games drive user traffic, but conversely are more difficult to break into, due to the competitive nature of the communities, as well the skill of their fellow runners.

Obviously, I was not able to solve any of these problems using a simple supervised learning algorithim, but by successfully training a model to predict in a supervised setting, I hope to learn more about what features were important for predicting run performance, as well as the scalability of the pipeline for future additions to the project.

The model as they were in my final run in my environment, have been saved in using `pickle`, and additionally CSVs have been added so you do not have to re-scrape the Twitch and Youtube data as I did. Also given the academic nature of the assignment, I spend some time explain my thinking process as we go through the process.

My only disclaimer is that I did not have enough time to properly visualize my data before I began to train my model - a big no-no, but I was working on a deadline and this was my first time working on a project end-to-end like this solo. Maybe in a future edit I will update with more visualization.

Tools and Data Source Rundown:

Data Sources:
Speedrun.com API
Youtube.com (scraped)
Twitch.tv (scraped)

Web Scraping Tools:
Selenium + ChromeDriver (for Twitch)
Beautiful Soup (for Youtube)

Analysis:
Pandas
Numpy
SciKitLean

Data Viz:
Matplotlib

Models:
Logistic Regression
GradientBoost
RandomForestClassifier
StackingClassifier (with Random Forests as the blender estimator)

