# Saving High Scores (writing files)
Write a program with three functions/procedures.

The first is a function, which should ask the user to enter five scores. The function should set up an array of five integers. It should loop, and ask the user to enter each score inside the loop. The function should return the array of scores.

The second is a function that takes the array of scores, and returns the highest score (using a find-max algorithm).

The third is a procedure, which should take the highest score as a parameter, and write it to a file called `highscore.txt`.

**Data flow table:**
```
getScores     IN    --
              OUT   scores() <- this is an array of scores

getHighest    IN    scores()
              OUT   high_score

writeHighest  IN    high_score
              OUT   --
```
