# ers_skill
algorithm that tests whether the card game egyptian rat screw is skill-based or luck-based


**large_gap**

ERS (card game) testing to determine whether it's luck-based or skill-based. 

Hypothesis: ERS is a luck-based game.

Process: develop ERS simulation in python. change likelihood of getting a slap in different models. run ERS games under each model 1000 times, gather results.

Data:

Model 0 shows games of ERS with no slapping: [239, 256, 256, 249]

Model 1 shows games of ERS where everyone has an equal chance to get the slap: [239, 261, 258, 242]

Model 2 shows games of ERS where player 0 has a 40% chance to get the slap, and everyone else has a 20% chance: [770, 77, 75, 78]

Model 3 shows games of ERS where player 0 has a 70% chance to get the slap, and everyone else has a 10% chance: [979, 10, 2, 9]

Model 4 shows games of ERS where player 0 has a 100% chance to get the slap: [998, 0, 1, 1]



Conclusion: ERS seems to be skill-based whenever a singular player has a substantial skill lead. Need further information concluding smaller skill leads.



**multi_player_gap**

ERS (card game) testing to determine whether it's luck-based or skill-based. 

Hypothesis: ERS is a luck-based game when multiple players have much higher skill than the other players.

Process: develop ERS simulation in python. change likelihood of getting a slap in different models. run ERS games under each model 1000 times, gather results.

Data:

Model 0 shows games of ERS where everyone has an equal chance to get the slap: [238, 234, 269, 259]

Model 1 shows games of ERS where the odds of getting a slap are 28/24/24/24: [377, 209, 215, 199]

Model 2 shows games of ERS where the odds of getting a slap are 30/30/20/20: [416, 417, 80, 87]

Model 3 shows games of ERS where the odds of getting a slap are 40/40/10/10: [497, 484, 7, 12]

Model 4 shows games of ERS where the odds of getting a slap are 30/30/30/10: [315, 369, 299, 17]



Conclusion: When two or more players have a similar skill level, they tend to win the same amount, therefore if skill is equal, the game is completely up to luck. Want more 
information concluding how small a skill gap actually affects the odds of winning a game.


**small_gap**

ERS (card game) testing to determine whether it's luck-based or skill-based. 

Hypothesis: ERS is a luck-based game when the skill gap between players is minute.

Process: develop ERS simulation in python. change likelihood of getting a slap in different models. run ERS games under each model 1000 times, gather results.

Data:

Model 0 shows games of ERS where everyone has an equal chance to get the slap: [252, 263, 276, 209]

Model 1 shows games of ERS where the odds of getting a slap are 26/25/25/24: [313, 228, 257, 202]

Model 2 shows games of ERS where the odds of getting a slap are 27/25/25/23: [316, 250, 248, 186]

Model 3 shows games of ERS where the odds of getting a slap are 27/25/24/24: [328, 243, 207, 222]

Model 4 shows games of ERS where the odds of getting a slap are 28/24/24/24: [341, 236, 200, 223]



Conclusion: Small amounts of skill difference does affect the outcome of the game, but not substantially. ERS is a skill-based game.

