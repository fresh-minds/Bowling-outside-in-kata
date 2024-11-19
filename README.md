# Bowling-outside-in-kata
This repo is meant for the bowling kata using a london-tdd-approach

## The Kata
We at Fresh-Bowl, are organising a weekly game of bowling.
When a Game is finished we receive a file from the bowling system and need to calculate the total scores by hand. As you can imagine this is time consuming and error prone.
And theirfore wish to change this process from a manual task to a more automatic task. Theirfore we wish that to have a system where we could give in a gamefile and process this to determine the winner for the game.
We also wish to store the game information for each person. So that at the end of the year we can give each players their average bowling score and how many games they won.

Processing means:

1. We extract the players data (name)
2. We calculate the score for each of the players.
3. Determine the winner of the game.
4. We than wish to store the game information for each player (separately) with the game information (Game date, score, end position).
   When there is already a file for the player than the information is added.
5. We Give back the name of the winner of the game.

## Input File:
FileName Game_2_2024_11_15 (foormat is Game_x_YYYY_MM_DD

Sjaak, 1,4,4,5,6,4,5,5,10,0,1,7,3,6,4,10,2,8,6
Piet,  10,1,3,8,2,10,0,0,8,0,7,2,8,1,10,10,10,6
Each Line starts with the players name, continuing with the pins rolled for each throw.

## Bowling Rules
The game consists of 10 frames. In each frame the player has
two opportunities to knock down 10 pins. The score for the frame is the total
number of pins knocked down, plus bonuses for strikes and spares.

A spare is when the player knocks down all 10 pins in two tries.
The bonus for a spare is the number of pins knocked down by the next roll.
For example if the input file starts with 4,6,4:
the 4 + 6 are in the same frame and add up to 10 so we have a spare.
We add a bonus of 4 (the third roll) to this frame as a result.

A strike is when the player knocks down all 10 pins on his first try.  The bonus
for that frame is the value of the next two balls rolled.

Special rule for 10th frame.

In the tenth frame a player who rolls a spare or strike is allowed to roll extra for the bonus score of the game.
For a spare this means 1 extra roll. For a Strike two extra rolls


