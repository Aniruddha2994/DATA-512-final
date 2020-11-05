# Efficient fighting styles in UFC
Aniruddha Dutta
License: [MIT License]()

### Motivation
UFC is world's biggest mixed martial arts event. There are a total of over 170 different martial art forms, each focusing on either grappling or striking, punches or kicks or a maixture of these integrated in one. In UFC, fighters from diverse backgrounds trained in different forms of martial arts battle for the championship in short rounds of 5 minutes. In these high intensity quick bouts, it is the fighting style and technique that determine the winner. 
This project aims at analysing the UFC matches data to determine the most efficient fighting styles in UFC. 

### Project Objective
Analyze the effectiveness of various fighting styles used by fighters in UFC
1. Exploratory data analysis
2. Devise a metric to quantify efficiency of a fighting style
3. Identify the most efficient fighting style across different weight categories and match time
4. Build a model that will predict who will win a match based on the fighter's fighting style along with other relevant features

The analysis will help in understanding which fighting style is efficient in a given match setting. It can also help provide an insightful comparison between champions from different era by analyzing their preferred style of combat.


### Data
The data for this project is scraped from ufcstats website. It is publically available at [Kaggle](https://www.kaggle.com/rajeevw/ufcdata).\
Additional information about data scraping can be viewed [here](https://github.com/WarrierRajeev/UFC-Predictions).

The data is a list of every UfC fight from 11 Nov,1993 till 7 Jun,2019. Each row is a compilation of both fighter stats. Fighters are represented by 'red' and 'blue' (for red and blue corner). The stats for both fighters include damage done by the fighter on the opponent and the damage done by the opponent on the fighter (represented by 'opp' in the columns), choice of fighting style, weight class of the fighter, etc. The target variable is 'Winner' which is the only column that tells you what happened.

<b>Column Definitions</b>
- <b>R_</b> and <b>B_</b> prefix signifies red and blue corner fighter stats respectively
- <b>_opp_</b> containing columns is the average of damage done by the opponent on the fighter
- <b>KD</b> is number of knockdowns
- <b>SIG_STR</b> is no. of significant strikes 'landed of attempted'
- <b>SIG_STR_pct</b> is significant strikes percentage
- <b>TOTAL_STR</b> is total strikes 'landed of attempted
- <b>TD</b> is no. of takedowns
- <b>TD_pct</b> is takedown percentages
- <b>SUB_ATT</b> is no. of submission attempts
- <b>PASS</b> is no. times the guard was passed?
- <b>REV</b> is the no. of Reversals landed
- <b>HEAD</b> is no. of significant strinks to the head 'landed of attempted'
- <b>BODY</b> is no. of significant strikes to the body 'landed of attempted'
- <b>CLINCH</b> is no. of significant strikes in the clinch 'landed of attempted'
- <b>GROUND</b> is no. of significant strikes on the ground 'landed of attempted'
- <b>win_by</b> is method of win
- <b>last_round</b> is last round of the fight (ex. if it was a KO in 1st, then this will be 1)
- <b>last_round_time</b> is when the fight ended in the last round
- <b>Format</b> is the format of the fight (3 rounds, 5 rounds etc.)
- <b>Referee</b> is the name of the Ref
- <b>date</b> is the date of the fight
- <b>location</b> is the location in which the event took place
- <b>Fight_type</b> is which weight class and whether it's a title bout or not
- <b>Winner</b> is the winner of the fight
- <b>Stance</b> is the stance of the fighter (orthodox, southpaw, etc.)
- <b>Height_cms</b> is the height in centimeter
- <b>Reach_cms</b> is the reach of the fighter (arm span) in centimeter
- <b>Weight_lbs</b> is the weight of the fighter in pounds (lbs)
- <b>age</b> is the age of the fighter
- <b>title_bout</b> Boolean value of whether it is title fight or not
- <b>weight_class</b> is which weight class the fight is in (Bantamweight, heavyweight, Women's flyweight, etc.)
- <b>no_of_rounds</b> is the number of rounds the fight was scheduled for
- <b>current_lose_streak</b> is the count of current concurrent losses of the fighter
- <b>current_win_streak</b> is the count of current concurrent wins of the fighter
- <b>draw</b> is the number of draws in the fighter's ufc career
- <b>wins</b> is the number of wins in the fighter's ufc career
- <b>losses</b> is the number of losses in the fighter's ufc career
- <b>total_rounds_fought</b> is the average of total rounds fought by the fighter
- <b>total_time_fought(seconds)</b> is the count of total time spent fighting in seconds
- <b>total_title_bouts</b> is the total number of title bouts taken part in by the fighter
- <b>win_by_Decision_Majority</b> is the number of wins by majority judges decision in the fighter's ufc career
- <b>win_by_Decision_Split</b> is the number of wins by split judges decision in the fighter's ufc career
- <b>win_by_Decision_Unanimous</b> is the number of wins by unanimous judges decision in the fighter's ufc career
- <b>win_by_KO/TKO</b> is the number of wins by knockout in the fighter's ufc career
- <b>win_by_Submission</b> is the number of wins by submission in the fighter's ufc career
- <b>win_by_TKO_Doctor_Stoppage</b> is the number of wins by doctor stoppage in the fighter's ufc career


