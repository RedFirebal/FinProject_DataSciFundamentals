# Final Project for Data Science Fundamentals - Sean, Jake D, and Charles

## Introduction

The purpose of this project was to give us expereince with finding, cleaning, querying, and analyzing a dataset to build upon the skills we have learned throughout the semseter. We were tasked with locating a dataset, creating and answering five research questions, applying a machine learning technique, and creating this documentation. After some deliberation amongst our group we settled on a dataset of video game sales from Kaggle. Following our decision be began to create our guiding questions and settled on these 5:
* Is there any correlation between best preforming genere and platform?
* How do the top sales of NA, JP, EU, and other differ from each other?
* Does year of introduction affect the sales and preformance of a game?
* Does having a well known publisher correlate to having good sales?
* Does platform affect the sales of a game?

As for applying a machine learning technique, we settled on investigating:
* Does a games release year predict its global sales?

## Selection of Data

### Dataset Overview
We chose our [dataset](https://www.kaggle.com/datasets/gregorut/videogamesales) both because of interest and due to the fact that the large amount of numerical data contained within would allow us to analyze our data without too much transformation. Our dataset has several categories:
<img width="1182" height="450" alt="image" src="https://github.com/user-attachments/assets/0eb7cc61-0bd3-4387-97c9-647e69c6189e" />
* The Ranking/Index
* The name of the game at said place
* The platform the particular game was released on
* The year of release
* The game's publisher
* The sales for North America (in millions)
* The sales for Europe (in millions)
* The sales for Japan (in millions)
* The sales for all other countries (in millions)
* The global/total sales overall (in millions)

### Dataset Cleaning

While our data was relatively clean, we still had about 2% (roughly 350 datapoints) of missing or N/A data. While much of this data was well enough down in the ranking to not have much of an effect on our final outcome, we opted to fill in a large chunk of this missing data by hand. The missing data was contained almost entirely in release year and/or publisher which are can be easily fact checked and filled in. By this effort did we bring the about 350 missing values down to 139 values, which is under 1% of our data. After bringing it to this point, we decided that our data was good enough to properly work with and went on to setting it up for analysis of our topic questions.

### Data Oddities

Our dataset does have a few oddities in it which we cant really fix or edit. The biggest oddity is that our data is missing sources from particular years, specificly 1979, 2018, and 2019. Some years also have very low numbers of logged releases which will likely affect our conclusions, likely not signifigantly but at least notably.


## Methods
### Packages

* Pandas
* Numpy
* Matplotlib

### Charting/Machine Learning Applied

* Bar Chart
* Line Plot
* Scatter Plot
* Linear Regression

### Specific Analysis Features

To make work on our dataset easier, we decided to break up our original dataset into several subframes in our initialization. While most of these subframes were not utilized, they were a great initial foray into our data. By setting these up, we were able to further understand what information our data contained, see several different ways to set up later frames, and have shorthands for particular data groups to look at when asking questions.
<img width="1113" height="361" alt="image" src="https://github.com/user-attachments/assets/1fcc574f-db62-4641-bdff-c7f7ec87ca1a" />



## Results

Here is what we discovered after working with our dataset for a while.

### Question 1 (Is there any correlation between best preforming genere and platform?):



### Question 2 (How do top sales differ by region?):



### Question 3 (Does year of introduction affect the sales and preformance of a Game?):



### Question 4 (Does having a large publisher size of released games correlate to having good sales?):



### Question 5 (Does platform affect the sales of a game?):

Understanding how a game preforms across platforms is relatively simple in concept. We first need to decide exactly what platforms we are comparing. For the purposes of our analysis, we decided to look at the 7th console generation (The XBox 360, the Playstation 3, and the Nintendo Wii) and compare games shared across these consoles would be placed into a shared frame.

<img width="763" height="201" alt="image" src="https://github.com/user-attachments/assets/f8b298eb-c88a-4e49-9c36-fd0b792c9c46" />

Then we generate a randomized list of names from this shared frame and produce shorthand frames per console containing only the information of these names.

<img width="586" height="319" alt="image" src="https://github.com/user-attachments/assets/0850241e-5088-40a5-b96c-dd41855128a1" />

After plotting this information, we can compare the sales of each game.
Example:

<img width="1511" height="1011" alt="Q5_Chart_Example" src="https://github.com/user-attachments/assets/ace1bec0-a47b-44c5-8269-1af9b9372da0" />



After making a few different generations of this chart, it has become abundantly clear that there is almost always some level of difference in preformance across platform. Considering that our data works in millions, every difference is usually in terms of thousands to hundreds of thousands of dollars. Notable differences tend to show up in every generation, showcasing that games tend to sell much better on particular platforms rather than noting similar sales across all platforms. This could be due to several factors ranging from audiances on particular platforms being attracted to certain aspects of a game to that particular platform offering a unique experience with a particular game. 


### Question 6 (Does a games release year predict its global sales?): 



## Conclusion
