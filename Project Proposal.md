# Make-or-Miss League

_Full Disclosure:_\
I have been having a tough time choosing a project for a myriad of reasons. There are instances where I have enough data (Formula 1 racing) but not sure what the question would be (how does qualifying result, pit stop numbers affect race result?). There are questions I find interesting (whether a golfer will make par or better or not) that don't have enough data. And then there are topics I like and have enough data (people's tastes in wine) that seem to have been classified to death with these sort of projects. Below I've settled on something that satisfies the requirements of the project so that I have something to propose but I do not find it particularly exciting as it is quite an unoriginal question and the data is dated, making the business case not as compelling. Over the next day or two, I will be looking to see if there are other feasible project ideas from above. I'm particularly interested in the F1 data, which is given by lap or by race result, and formulating a classification question around it. 

## Question
In recent years, the NBA has become an increasingly "make or miss" league. This means that despite all the strategy that may go into a game, it may ultimately be decided by whether a team or player makes his shots. In this module, I will explore this base question and which features contribute most to a make/miss. I hope to provide valuable insight on how not only the shot distance but also other factors such as time in the game, defender proximity, and time that a ball is held, can affect the likliehood of a shot going in. 

## Data
I have found a dataset of 128K+ rows that I believe has every shot taken in the 2014-2015 NBA season. Each row contains a single shot taken by a player, the distance of the shot, actions taken before the shot, the time in the game, and closest defender/distance. I may add data in the form of dummy variables to categorize the different distances of two point shots. Naturally, I expect two point shots to have a higher likelihood of being made than three point shots but it will be interesting to explore how long 2s (say 18-22 feet) compare.   

## Tools
I anticipate using pandas and possibly SQL for EDA and data cleaning. Other python packages such as sklearn will be used for the classification models. Seaborn/Matlab will be used in some respect if just diagnostically. I really enjoyed using Tableau last module so would like to bring that in if possible. 

## MVP Goal:
I anticipate to have an initial read on which factor contribute most to a successful shot. 




