# 2024 General Elections Prediction
This project attempts to predict the 2024 General Election outcome using Jim Albert's Bayesian framework that can be accessed at https://learnbayes.blogspot.com/2008/10/how-many-electoral-votes-will-obama-get.html. 

The state-level polling data is available on fivethirtyeight.com: https://projects.fivethirtyeight.com/polls/president-general/. For each state, I use the most recent polling result up to 10/30/2024, i.e. the poll that has the most recent end date. Some less competitive states have no publicly available poll results (e.g. Alabama, D.C.), so I manually input the win probabilities as 0 if they are red states and 1 if they are blue states. 

After elections update: I correctly predicted that Trump would win, however, he won with more votes than I predicted. There could be several reasons for this: 
* States are assumed to be independent. In reality, states that are geographically close or share common borders can affect each other in voting. 
* Some pollsters lean towards a certain candidate/party and the quality of polls differ. To improve, one could add a weight of poll qualities when we select the most recent polls, and select the highest quality polls. 