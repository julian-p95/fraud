# fraud

# tennis fraud

This project is designed to analyze tennis match data and detect potential instances of fraud or match fixing. The data is sourced from a CSV file and contains information on matches, players, and their winning probabilities.

The project involves data cleaning, exploration, and modeling. First, the data is cleaned and filtered to identify matches with significant changes in the winning probabilities of the players. These matches are then further analyzed to identify potential fraudulent activity.

Data
The tennis data is stored in a CSV file located at data/tennis.csv. The file contains the following columns:

match: A unique identifier for the match.
id: A unique identifier for the bet placed on the match.
année: The year in which the match took place.
P_gagnant_début: The initial probability of the winning player before the match started.
P_gagnant_fin: The final probability of the winning player after the match ended.
perdant: The name of the losing player.
gagnant: The name of the winning player.
Usage
To use the project, simply run the Jupyter notebook tennis-fraud-detection.ipynb. The notebook contains all the code needed to load and analyze the tennis data.

Results
The project identifies several players with potentially fraudulent activity. These players are identified based on the significant changes in their winning probabilities and are further analyzed using a statistical model to determine the likelihood of fraud.

The project's output is a list of the most suspicious players and the probability that they were involved in fraudulent activity. The results can be found in the results folder.


# Analysis of U.S. Election Data Using Benford's Law
This repository contains Python code that analyzes the results of the 2016 U.S. Presidential Election in three states (Wisconsin, Michigan, and Pennsylvania) using Benford's Law. The code was developed as part of a data analysis course.

Background
Benford's Law is a mathematical law that states that the first digit of many naturally occurring numbers is more likely to be smaller than larger. For example, in a large data set, the digit 1 should be the first digit about 30% of the time, and the digit 9 should be the first digit less than 5% of the time. Benford's Law has been used to detect fraud in financial accounting, and has been applied to election data to detect irregularities.

Data
The data used in this analysis was obtained from the MIT Election Data and Science Lab. The data includes the vote counts for the three candidates (Trump, Clinton, and Stein) in each county in Wisconsin, Michigan, and Pennsylvania.

Analysis
The code in this repository performs the following analysis:

The data is loaded from a CSV file and filtered to only include counties in Wisconsin, Michigan, and Pennsylvania where each candidate received at least 10 votes.

The second digit of each candidate's vote count is calculated and counted for each state.

The frequency of each second digit is compared to the expected frequency according to Benford's Law, and the results are plotted in a bar chart.

The distance between the observed frequency and the expected frequency is calculated using the Euclidean distance formula.

A simulation is performed where a random sample of 220 vote counts is generated using the expected frequency from Benford's Law. The distance between the simulated frequency and the expected frequency is calculated, and the number of simulations where the distance is greater than or equal to the observed distance is counted.

The proportion of simulations where the distance is greater than or equal to the observed distance is calculated, and this is used as a measure of the plausibility of the data.

