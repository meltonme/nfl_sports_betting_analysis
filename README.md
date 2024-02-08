# NFL Sports Betting: An Analysis of Factors that Affect how Sportsbooks set Game Spreads and Over/Under Totals

### Repository Overview
- All data used in this analysis can be found in the "Data" folder
- Individual files for each visualization and summary can be found in the "Output Data" folder
- The script used to aggregate the data can be found in the folder labeled "NFL Betting Analysis"

### Background 
With the legalization of sports betting spread across the country rapidly starting in 2018 when the Supreme Court overturned the Professional and Amateur Sports Protection Act (PASPA). The law effectively made sports betting legal in Nevada and a few other states. With the upcoming Superbowl LVIII (58); our project will focus on how various factors pertaining to how sportsbook set game spreads and over/under total.

## Technology Used and Data Cleaning Process - Miranda Melton

### Data Location 
The original datasets were found in a Kaggle Notebook called "NFL Scores and Betting Data" ("https://www.kaggle.com/datasets/tobycrabtree/nfl-scores-and-betting-data"). 

This data included game results since the 1966 season with betting odds information since 1979. Additional datasets included weather information from NOAA data and NFLweather.com Betting data was used from http://www.repole.com/sun4cast/data.html for 1978-2013 seasons. Pro-football-reference.com data was then cross referenced for betting lines and odds as well as weather data. From 2013 on betting data reflects lines available at sportsline.com and aussportsbetting.com.

The Kaggle Notebook included 3 data sets 
- nfl_stadiums (includes data on location, climate, type, capacity, etc)
- nfl_teams (includes data on historical team names and division/conference placement pre and post 2002)
- spreadspoke_scores (includes game results, spead and over/under information, etc)

### Technology Used 
- Jupyter Notebook
- Python
- Pandas
- MatplotLib
- Numpy
- Pathlib
- Scipy.stats
- Seaborn
- Warnings.filterwarnings

### Cleaning Process 
- Upload the .csv files
- Merge the nfl_stadium and nfl_teams to create a DataFrame called "team_stadium_merged"
- Change the names of the columns to make them easier to read
- Create new DataFrame called "renamed_team_stadium_merged"
- Export that data into a .csv file called "new_team_stadium_data"
- Add any missing relevant data
- Drop columns that were not needed for the analysis
- Reformat the 'Stadium Capacity' numbers so that they match to make analysis easier
- Locate and drop duplicates
- Locate and drop un-needed columns


## Stadium and Team Summaries 

## Stadium Summary 

### Quick Facts 
- There are 120 stadiums that have historically be used by the NFL
- Stadiums can be found mostly in the Unitied States with a small percentage located in other countries such as England, Germany, and Mexico
- This data set includes college stadiums which have been used as a team's first location or as a temporary location during a stadium renovation

### Stadium Capacity 

74 stadiums (~62%) have a seating capacity of 50K to 75K. On both extremes, only 4 NFL stadiums have a seating capacity of less than 25K and only 2 NFL stadiums can sit between 100K to 125K spectators. 

![Stadium Capacity Ranges](Output-Data/Stadium Capacity Ranges.png)

