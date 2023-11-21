# Tennis kata

Tennis is a ball and racquet game that is scored using the scoring 0, 15, 30, 40, and A. \
A player must score at least four points in total and two more than their opponent to win. 
When the points are four, and the scores are equal, then the 
score is 'deuce' (40:40). When the points are four or more, and a player has one point more than their opponent, then the score is 'advantage' (A:40).

We want a program that can be used to score a game in real time. To begin with, we're going to need a way to update the score when a player wins a point, see what the current score is after each service, and see if their is a winner based on the current score and the rules above.


## Feature 1 - Winning a Point Increases Score Correctly
As a library user \
I want the score to increase when a player wins a point \
So that I can display the current score correctly.

- Given the score is 0:0 \
When the server wins a point \
Then the score is 15:0 
- Given the score is 15:15 \
When the receiver wins a point \
Then the score is 15:30
- Given the score is 30:30 \
When the server wins a point \
Then the score is 40:30


## Feature 2 - Winning Points are Scored Correctly
As a library user \
I want the winning point to be scored correctly \
So that I can display the winner

- Given the score is 40:30 \
When the server wins a point \
Then the server should win
- Given the score is 0:40 \
When the receiver wins a point \
Then the receiver should win

## Feature 3 - Deuce and Advantage are Scored Correctly
As a library user \
I want deuce and advantage to be scored correctly \
So that I can display the score correctly

- Given the score is 40:40 \
When the server wins a point \
Then the score is A:40
- Given the score is 40:40 \
When the receiver wins a point \
Then the score is 40:A
- Given the score is A:40 \
When the server wins a point \
Then the server should win
- Given the score is A:40 \
When the receiver wins a point \
Then the score is 40:40

  
## Expectations
- DDD are concepts modeled ?
- unit tests ?
- git history ?
- (im)mutability ?
