# NFL-Win-Probability-Model

## Project Description

The main aspect of this project will consist of a machine learning model in Python that will predict which team will win each NFL game on a week-by-week basis for the
current NFL season. Using historical data, a model (either logistic regression or XGBoost) that predicts the winner of a given matchup will be fit. Then, once the model 
has been fit, for every matchup in an upcoming NFL week, the data for both teams in the game will be passed into the model and it will produce the probability that each 
team wins the game. My model's predictions can be juxtaposed with betting market odds and after the games are played, my model's predictions can be juxtaposed with the 
actual outcomes.

The initial stages of the project will consist of creating datasets containing all the historical data for every team over the last several seasons. Then, after the data
has been collected, the chosen model will be fit and adjusted until it has achieved a good fit.

After the model has been constructed, a profile for each NFL team season will be constructed, based their performances so far this season. Ideally, there will be about two
months worth of data for each NFL team this season. Then, for each upcoming week and each matchup that week, the profiles for the teams playing each other will be passed
into the model and the model will predict the winner and ideally the probability of that team winning. This is to help distinguish between games the model expects to be 
close and games the model expects to be blowouts, in order to make comparisons to betting markets and contextualize outcomes.

The end goal will be to compare by model's predictions with the actual outcomes, as well as seeing if my model is more reliable than if you went according to the odds given
by major betting companies.

## Goal:

Successfully predict the winner of NFL games, based on each team's recent performance and team architecture (i.e. players, coaches, home or away, etc.)

## Data Collection

Historical game data can be collected using the nflfastpy package, which contains play-by-play descriptions and statistics for every NFL game since 1999. Using pandas, any
relevant information can 

Websites such as https://www.pro-football-reference.com contain additional historical information, as well as lists of players and coaches and their historical profiles on
a year-by-year basis. This will help establish baselines for evaluating a team's roster and coaches. For example, say a team had a quarterback that made the Pro Bowl that
year. A potential predictor to include in the model could be elite_qb, a binary outcome that equals 0 if the quarterback is not elite, meaning they didn't make the Pro
Bowl, and 1 if they did. Then, the model can account for the affect of an elite quarterback on a team's win probability.

Additionally, as an avid NFL viewer and someone who played football throughout my childhood, my own opinions collected from watching games will also be incorporated into 
the model (ex: Do I think this player is actually good, despite his statistical profile not showing that at the moment?) This is subjective, but it is also where my own
insights can help set my model apart from other models, as it will be based not just in statistics, but in an understanding of the sport itself.

Some data that will be collected include: roster quality, coach quality, setting of the game (i.e. home or away, weather), injuries, rest days between games, performance
over the prior weeks, and advanced statistics over the past couple games (ex: offensive EPA, third-down conversion rate).

T
