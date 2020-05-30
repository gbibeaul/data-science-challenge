# Datascience test project

This is a test datascience project I did mainly to give a shot a data science. The goals were to run statistical analysis on a soccer game data set and to build a prediction model of which team would win given on it's past history.

open up [The Notebook](soccerNotebook.ipynb) to see results

### Statistical analysis:

In pandas the following exploratoty analysis were ran:

1. average number of goals for the home team
1. average number of goals for the away team
1. histogram of the number of total goals we can see in a gam
1. home team’s win percentage
1. Which country has scored the most goals in FIFA events (qualifiers, cups, etc.) since 2010

The following predictions were attempted:

1. Which country is most likely to win the next FIFA even
1. Is the difference between the home and away teams average goals statistically significant

The following model was trained:

1. predicts the probability of a team winning a game given its opposing team and where they’re playing

the model was trained with the following method:

- [x] kept only fifa games on non neutral grounds since we are interested in location
- [x] calculated then the ods of each country to win at home and away
- [x] merged original data frame with ods dataframes to match teams with their ods of winning away/home
- [x] ran logistic regression and trained a model on 75% of the data set

the model's accuracy was 65% in the end.

### Next steps:

- add a team vs team ods column on both away and home teams.
- sklearn.MLPClassifier tests
