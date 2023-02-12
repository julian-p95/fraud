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
