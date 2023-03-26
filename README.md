# soccer
### A probabalistic soccer game

This is a program to simulate a soccer game between 2 teams. Each team is composed of 3 players: a goalie, defender, and forward.  They are arranged on the field in the following way:
Goalie A - Forward B - Defender A - Defender B - Forward A - Goalie B
Each player has a randomly generated skill level between 40 and 70% at the beginning of the game. This skill level is the success-rate of any action carried out by that particular player.
Each position attempts to pass to the next player on their team.  Their attempt succeeds with a rate equal to their skill level.  If it succeeds, the next player on their team receives the ball.  If it fails, the opposing player that is closest to them receives the ball.  If the forward succeeds, their team receives one point and the opposing goalie starts with the ball.  Each failed or successful score attempt results in the opposing goalie receiving the ball and trying to pass to the defender.

At the start of the game, a random goalie is chosen and tries to pass to the defender. Terminate the game when one team hits 3 points.

The program output will emulate a sports caster’s description of the game. For example:
```
Goalie A attempts to pass to defender A.  
Defender A successfully receives a pass!
Defender A attempts to pass to forward A. 
Defender B intercepts the pass!
Defender B attempts to pass to forward B. 
Forward B successfully receives a pass!
Forward B attempts shot on goal A! 
GOAL!  Team B’s score is 1. Team A's score is 0. 
Play continues
Goalie A attempts to pass to defender A.
```
