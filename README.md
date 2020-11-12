# Toxic Behaviour in Online Gaming
Aniruddha Dutta
License: [MIT License](https://github.com/Aniruddha2994/DATA-512-final/blob/main/LICENSE)

### Motivation
The popularity for online competetive gaming is increasing exponentially. Billions of people worldwide get together to play online games and some of theme have even made a career out of playing games called 'pro-players'. The rise of gaming industry has opened up new career options such as professional players, viddeo-game streamers, game casters and many more. It has given birth to a fascinating online social community and gaming culture. But there are some major problems that the gaming community is facing, one of them is the issue of toxic behaviour. Players competing with eachother in online games often use profane and toxic language in the heat-of-the-moment or as strategy or simply to vent their frustration. Communication channels might be abused to harass and verbally assault other players, which negates the very purpose of entertainment in games by creating a toxic player-community. As a gaming enthusiast myself, I wish to analyze the toxic behaviour in online gaming and how it affects mental health of players.

### Project Objective
Analyze the Toxic behaviour in online gaming and its impact on mental health
1. Exploratory data analysis of mental health data of online gamers
2. Classify in-game chat messages/comments into different toxicity category
3. Explore impact of comments on mental health

### Data
###### 1. Dota 2 Game Chats:
For this project, I will focus on ingame chat data for Dota 2 — video game by Valve, one of the most popular eSport discipline. A single match of Dota 2 is played between 10 players who are divided into two teams (Radiant and Dire) of 5 players each. Dota 2 enjoys one of the largest numbers of online players worldwide. Though data is for a specific game, it is a fair representation of the MOBA(multiplayer online battle arena) gaming genre which is the most popular and competetive online gaming genre. 

This dataset contains chat messages from Dota 2. It contains chats of almost 1M matches from public matchmaking (when players are selected by the game server at random with about the same skill level).
It is publically available at [Kaggle](https://www.kaggle.com/romovpa/gosuai-dota-2-game-chats).\

<b>Column Definitions</b>
- <b>match</b> Match index (primary key)
- <b>time</b> Game time when the message was sent
- <b>slot</b> Player slot (0–4 for Radiant (Team A), 5–9 for Dire (Team B))
- <b>text</b> Text of the message

 
###### 2. Online Gaming Anxiety Data:
This dataset consists of data collected as a part of a survey among gamers worldwide. The questionnaire asked questions that psychologists generally ask people who are prone to anxiety, social phobia, and less to no life satisfaction. The questionnaire consists of several set of questions as asked as a part of psychological study. The original data was collated by Marian Sauter and Dejan Draschkow.
It is publically availaible and can be downloaded from [here](https://www.kaggle.com/divyansh22/online-gaming-anxiety-data).\

<b>Column Definitions</b>\
The data consists of 55 columns that correspond to every question asked in the survey questionnaire. Most of the columns correspond to different scoring criteria used in psychology like GAD (General Anxiety Disorder), SWL (Satisfaction with Life) an and SPIN (Social Phobia Inventory) scores. There are a few generic questions about where the people are born and why do they lay online games etc.
