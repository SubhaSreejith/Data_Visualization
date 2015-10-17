Summary:

I chose the Baseball dataset to build an effective visualization from a list of over 1100 Players. 

In order to uncover facts from this dataset, the reviewer is presented with a graph of handedness vs batting average to substantiate my hypothesis that on an average left handed batsmen have a higher batting average than right handed and switch batsman. 

In the box graph the average of L is  better  than B and R .The outliers are removed in the boxplot depicted using R.
In the d3.js visualization graph the average of L and B is same and R is lesser than them. Here the outliers are not removed.

From R and statistical modelling I could clearly say that Lefties are best performers than Righties and switch.

The x and y axes indicate handedness and Batting average  . 

Design

I chose bubble chart because it has the ability to highlight the players when the mouse move over happens.
I initially focussed on BMI analysis to see if the highest run takers have exhibited a certain body type. There is roughly about 20 pounds that reside in which thereby changes the striking capability based on their posture and the angle the ball is being pitched. But it is very unlikely that someone who is tall would be able to hit the homerun off. 
Then I thought definitely the physical characteristics especially height and weight helps the hitter most easily maximize their potential to hit.So, in the plot I chose to map the variables related to x and y axis. Based on their height and weight I ordered them to see the total runs they hit. This will help to audience to get a sense of relative heights when they look at the heights on the yaxis. I simply chose the weight on x axis based on my intuition. I also put the home runs on z axis to understand their total runs without scrolling over each one individually. I was not able to conclude that a good hitter will have good batting average and certain type of body composition.. 

I started to think in the direction that a Individuals performance is considered greately based on the batting average. I decided to look a bit more in to this to see if the highest batting average is exhibited by a left hander or a right hander or both.

I used bar chart to visually show the difference in average and plotted average of Batting averages against the Handedness.
Here the entire data set is chosen and performed the study in R and also used my learning from R to show the conclusions in d3.

From the top 10 values, I could see that a left hander has the most batting average (7 out of 10) compared to a righty or a switch player.

Initial Feedback 1

I first took the graph to my Dad and gave him an overview of nanodegree and the project objective.He was totally confused to see all the players and all cluttered in the graph. I had to show him the bubbles every time and he was not able to relate how many runs have they hit  and also to see who had hit without scrolling over and since a lot of data, the clarity was missing.
He was not clear on: 
Overlapping circles.
Unable to find the Top hitters.
Not interactive and he was just not interested in the view

Design Change 1:

I took the top 50 players based on the home run hitters and also colour the legend by player names so there was a way to tell who has hit what.I sort the players by the name and total home runs hit by the players.I also realized that the axis had been sorted by categories and felt the representation was not that great. 

Feedback 2

I showed the graph to my husband and thought he will be able to help since he is a baseball fan. He scrolled down a bit looking at the player names . I realized that he didnot understand what I was going for and so explained him the objective of the project. At first I had not provided the  tool tip had only the name attribute. With that design he was not able to make up anything from the chart and I had to explicitly tell him the objective of my analysis.Secondly, he was trying to locate the top 10 players and told me that it would be effective to add some toggle functionality that takes to the exact scatter bubble in the chart.

Design change 2:

I then included the other attributes to the tool tip so that when the audience brings the mouse over they can compare and know the batting characteristics. Secondly I also included the on click functionality to legend below to show each player name which will make the audience understand the chart without using a mouse over.I decided to make the legend bit more interactive , While I started to work I also learned to get the variables I need to in response to mouse hover.

Feedback 3:

I showed to my friend. She doesnt know much about baseball but she could give me good review comments.
She liked the colors and the mouse over feature and also could see the extra info. She said as an audience she would like to see how many right handed batsman and left handed batsman were there and also see who performed well .
She also gave me another of option of looking at players BMI, height and weight and compare against the home runs and study the findings.


Udacity Feedback:

Here are some ideas that you can look into:
Can we prove the common wisdom that left handed baseball players are better at batting?

Based on the available data set of 1157 baseball players you could look at batting average score by player where batting average – determines the skills of players at batting and is an excellent indicator for individual performance.
Look at the distribution by handedness for batting average and their mean value
look at the Top 10 players by batting average.

Udacity reviewer was still not able to gather any insights and he suggested to again explore the data.

I again got 2 review comments:

1. Look at the distribution by handedness for batting average and their mean value (by handedness)
2. look at the Top 10 players by batting average (you will notice that from top 10 there are 7 left handed batsmen. This is more appealing to the viewer, because now he/she would be to conclude that lefty's are in general good )
Using both the questions above give a compelling story to the viewer.

I had a chat with my coach and she suggested to refine the representation so that they are explanatory in nature.

Index.html Final story:

Based on my discussion with udacity coach I initially developed the visualizations in R to boil down on the factor that on an average left  batsman are considered to be good . The population contains majority of records for R batsman(64%) followed by L batsman(27%) and switch (9%)

I made Descriptive title  slategray as black was taking some focus off the visualization. The axes font are set to Garamond to make it easily readable. I included the legend to the bottom and included all players and left the default color scheme. 

I plotted a graph of Average of Batting averages against Handedness and observed Average of L batsman  is significatly above the average of R players and B players.

The Left handed batsman exhibited an average of 0.252
The Switch batsman exhibited an average of 0.239
Right Handed batsman exhibited 0.238

It’s fairly true that in major league baseball left-handed batters , on average, hit better than their right-handed counterparts. 

