# fpl_model

This repository contains a set of models built for Fantasy Premier League (FPL):
- [draft_picks.ipynb](https://github.com/amirgrunhaus/fpl_model/blob/main/draft_picks.ipynb): this notebook contains a model that optimizes the draft player-selection process by ranking the best player picks per draft round. For every draft round, the algorithm ranks 10 players per round (for a 10-manager league), based on statistics from the 2021-22 season. The model also returns ideal FPL Draft teams for every used statistic.

- [pl_predictions.ipynb](https://github.com/amirgrunhaus/fpl_model/blob/main/pl_predictions.ipynb): this notebook contains a ML Linear Multiple Regression model that predicts how many points a player will score for a specific gameweek during the 2022-23 PL Season based on data dating back to the 2017-18 PL Season. The model also recommends an ideal team for the upcoming gameweek based on predicted total points.

- [fantasy_ideal_team.ipynb](https://github.com/amirgrunhaus/fpl_model/blob/main/fantasy_ideal_team.ipynb): this notebook contains a model that creates 3 ideal FPL teams. The teams are based on each player's last season total points, PP90min (points scored per 90min played), and ROI (Return on Investment - how many points the player returned for every £1 invested in them). 

Supporting notebook:
- [data_update.ipynb](https://github.com/amirgrunhaus/fpl_model/blob/main/data_update.ipynb): this notebook updates the training data weekly for the gameweek points prediction model. 

In the [data directory](https://github.com/amirgrunhaus/fpl_model/tree/main/Data), you can find the following data:
- **Player data for each gameweek since the 2016-17 PL season** - one folder with various csv files for each season (credits to [vaastav](https://github.com/vaastav/Fantasy-Premier-League) for scraping data from the FPL site every week).
- **training_data.csv**: original training data set containing data since the 2016-17 PL season (credits to [solpaul](https://github.com/solpaul/fpl-prediction)).
- **training_data_updated.csv**: updated training data with player data for each new 2022-23 PL season gameweek.
- **cleaned_merged_season.csv**: player data for each gameweek since the 2016-17 PL season merged (all individual folders merged).
- **master_team_list.csv & teams.csv**: team names and IDs (global and for each season).
- **remaining_season.csv**: dataset with each player's remaining fixtures in the current season.

**There's some extra data in the directory, however, the data specified above is the most relevant and what I use in the notebooks.*

I'm currently working in new notebooks and will be updating the repository weekly.
