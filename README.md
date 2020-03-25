# NCAA March Madness Machine Learning
### Daniel Valdes, Thomas Byrne, Pete Sheldon, Jack Bitcon
<<<<<<< HEAD
![bracket](https://www.ncaa.com/sites/default/files/public/styles/original/public-s3/images/2019/04/09/ncaa-tournament-bracket-2019-scores-games-virginia-texas-tech.png?itok=0E3VNWmI)
=======

(https://www.ncaa.com/sites/default/files/public/styles/original/public-s3/images/2019/04/09/ncaa-tournament-bracket-2019-scores-games-virginia-texas-tech.png?itok=0E3VNWmI)
>>>>>>> cb143977347a213c03d06a36fdb482502f7b0435

Data sourced from: https://www.kaggle.com/c/march-madness-analytics-2020/overview

64 teams participate in the NCAA tournament each year. The tournament bracket is divided into four regions (North, West, East, and South) that have representation from all of the nation's 32 conferences. There are six rounds of knockout games in which the winner advances to the next round and the number of partcipants is halved each time. The champion will have effectively won six games at the end of the tournament. It is a notoriously difficult tournament to predict and the odds of filling out a perfect bracket have been estiamted at 1 in 9.2 quintillion. This project is an attempt to grapple with the Madness and apply machine learning techniques to previous years to try and build a model that can predict winners reliably.

For machine learning purposes there are multiple approaches we can attempt: 

1. Set our target variable *Y* to Number of Wins and test different independent variables influence on a scaled *Y* (**Multiple Regression**)

2. Divide teams into different groups that denote success and try to classify them (**K Nearest Neighbors**) based on the features we select. This can be achieved by counting the number of wins in the tournament.

1st/2nd Round Exit: Wins <= 1 \
Sweet Sixteen: Wins = 2 \
Elite Eight: Wins = 3 \
Final Four: Wins = 4 \
Semi-Finalists: Wins = 5 \
Champion: Wins = 6

3. Model the problem using **Logistic Regression**. To use logistic regression, we need to frame our question in a way such that a binary answer of *1* or *0* (Yes or No) makes sense. For example, we can ask "Did team X advance to the next round?". We can then pass a vector for team X containing our selected features. Those teams that return a 1 advance to the next round and the simulation is run once more.
