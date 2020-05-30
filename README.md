# Predicting the Results for the remaining fixtures of the postponed Premier League 19-20 season
Due to the COVID-19 pandemic, a lot of football fans, like myself, have been upset due to the cancellation of the Premier League (and other leagues of course). Since I had a lot of free time now, I decided to try and predict the remaining fixtures of the English Premier League if it would have continued. <br>
<br>
I am aware now it might continue from June onwards but you can consider these results as what could have been if the league had continued without halt.<br><br>
I am only considering the performances of each team in the League so far, and not each player's performance. Please view the Assumptions to get a better understanding of what I'm getting at.<br>

If you are not interested in looking at the code, but just the final result, you can either scroll down or refer this blog post - https://medium.com/@joshanbabu96/predicting-the-remaining-premier-league-19-20-fixtures-1f41feaaf20f <br>

## Assumptions

These are the following assumptions:

1. <strong>Injury issues</strong><br>
If a player would have gotten injured in an upcoming fixture or missed many previous games due to injury but would have made it back by 11th March, that would certainly affect how the team would play, and thereby the result.
<br>However, I did not consider any of these changes.

2. <strong>Manager changes</strong><br>
Any possible manager changes which could affect playing styles of games will not be taken into account.
<br>A team’s performance is based on their overall performance in the league till now. So, if there was a manager who joined in between and changed the results thereafter, that doesn’t change how the team has been viewed.
<br>For instance, Carlo Ancelotti joined Everton on 21 December 2019 after which they have had much better results (5 wins out of 11 games as compared to 5 wins out of 18 games). Although they are playing better now, I have considered their pre-Ancelotti performance as well to determine where they stand in the league.

3. Any possibility of changes due to <strong>outside competitions</strong> (Champions League, Europa League, FA Cup, etc.) are also not taken into account<br>

4. Any <strong>tactical changes</strong> any team might perform in a game will also not be taken into account.

5. The difficulty for each match for each team is taken from the <strong>Fixture Difficulty Ratings (FDRs)</strong> from the Fantasy Premier League page.<br>

6. <strong>Rounding off numbers</strong><br>
There is obviously a lot of Math involved and the final scoreline can end up being something like 1.333–2.866 or similar. I was initially going to do a simple rounding off but I realized that a team with 2.8 goals doesn’t mean they would score 3 goals in a game but 2.99 means that they probably could. So, I set the limit at 0.9. If it is greater than 0.9, it will be rounded off to its ceiling value, else it will be the floor value.
    <br>Example:<br>
    1.333–2.866 = 1–2
    <br>0.95–1.1 = 1–1
    <br>2.90–2.91 = 2–3
