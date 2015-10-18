Summary:

I chose the Baseball dataset to build an effective visualization from a list of over 1100 Players. 

In order to uncover facts from this dataset, the reviewer is presented with a graph of handedness vs batting average to substantiate my hypothesis that on an average left handed batsmen have a higher batting average than right handed and switch batsman. 

I also compared the avg vs the home runs by handedness and it seems majority of the people who have batting average close to the overall batting average (0.245) have scored less home runs. L,B or R  cannot be claimed good performers based on this.

In the box graph the average of L is  better  than B and R .The outliers are removed in the boxplot depicted using R and d3.

From R and statistical modelling I could clearly say that Lefties are best performers than Righties and switch.

The x and y axes indicate handedness and Batting average  . 

Design


I initially focussed on height,weight analysis to see if the highest run takers have exhibited a certain body type. There is roughly about 20 pounds that reside in which thereby changes the striking capability based on their posture and the angle the ball is being pitched. But it is very unlikely that someone who is tall would be able to hit the homerun off. 
Then I thought definitely the physical characteristics especially height and weight helps the hitter most easily maximize their potential to hit.So, in the plot I chose to map the variables related to x and y axis. Based on their height and weight I ordered them to see the total runs they hit. This will help to audience to get a sense of relative heights when they look at the heights on the yaxis. I  put the home runs on z axis to understand their total runs without scrolling over each one individually. I was not able to conclude that a good hitter will have good batting average and certain type of body composition.. 

I started to think in the direction that a Individuals performance is considered greately based on the batting average. I decided to look a bit more in to this to see if the highest batting average is exhibited by a left hander or a right hander or both.

I worked extensively on R charts and also developed many plots including the one using plotly in R. 

https://plot.ly/~SubhaSreejith/35/batting-average-vs-handedness.embed

https://plot.ly/~SubhaSreejith/49/batting-average-vs-home-runs.embed

I also used python coding to support the statistical analysis oon the data.Finally I worked on the d3 coding from the understanding I gained from R and statisical test.

I have attached the R code, python code and also the d3 visualizations.

Initial Feedback 1

I took the design to Udacity coach and she gave me feedback to spend some time exploring the dataset, in a similar way to the Explore and Summarize Data project. 
She encouraged me to use Python or R (if more comfortable with those than with dimple or d3) to explore the data, making plots and trying ideas out. Make a whole load of different plots, exploring ideas. Make notes on the stories that I discover, and what seems to be effective or ineffective in communicating those stories. She asked me to not limit myself to the story about lefties .

Design Change 1:

I began my analysis with discovering  the distribution of handedness which depicted out of 1157 players the majority (64%) of players are right handed.27% of them are left-handed and remaining are 9% are both.
With the aim of arriving at best players, I drew the correlation graph which helped me to look in to the parameters height and Home runs against the batting average.
Even though height vs average correlation is within the acceptable range, in reality we see there is no linear relationship. This could be due to the fact that a small change in the height need not have any impact on the batting average.Since no linear relationship in this , I excluded the relationship to reach  any valid conclusions.
Then I looked at Batting Average vs Home Runs .From the graph it is clear that for the majority of high averagers the home runs scored is less . This is very evident for L and B but for R  there are some insatnces of high average when the home run is more.
I looked at the Batting avg vs handedness and I could see a slight difference in their bating nature from which I said L and B are better performers than R.

Feedback 2

I showed my work and received few more inputs and asked me to look at more data points - 
- In the ggpairs plot,  there was a single outlier in terms of batting average. She asked me if this player a baseball superstar? Is their performance important when considering all batting averages, or are they an outlier to be ignored?
- In the R file, the final boxplot seems to show that left-handers have a far wider range of batting averages than right-handers. Is that because there are more left-handers in the sample? Is it because right-handers are very uniform in their performance?
- How many 'switch' players are there in the dataset? Are they more similar to right- or left-handers or are they simply different?

Design change 2:

I eliminated the 0 batting average players as after research I felt these 0 average people might also be the pitchers who rarely get a chance to play.In Major League Baseball, the designated hitter is a hitter who does not play a position, but instead fills in the batting order for the pitcher.Hence the 0 batting averages might be for pitchers.
Their average doesnot have any significant role as they do not even bat.In my analysis since I am interested in knowing the batting average of an individual to analyse their performance and to which category of handedness they belong. Since I am interested in knowing actual hit on the bat and so excluded the 0 batters from my data and was able to say that the average of left handers seem higher of about 0.252 as compared to Both handed batsman of 0.239 and right handed batsman of 0.238.

Feedback 3:

Charlie liked the analysis and also suggested that I look in to the statistical test . She asked me to think if there is a meaningful practical difference as well as a statistical one? Would it be worth also testing for effect size?


Index.html Final story:

The population contains majority of records for R batsman(64%) followed by L batsman(27%) and switch (9%)

I plotted a graph of Average of Batting averages against Handedness and observed Average of L batsman  is significatly above the average of R players and B players

https://plot.ly/~SubhaSreejith/35/batting-average-vs-handedness.embed.

The Left handed batsman exhibited an average of 0.252
The Switch batsman exhibited an average of 0.239
Right Handed batsman exhibited 0.238

I rejected the the null hypothesis which asserts that the means of the two samples are identical.From the R graph I saw that average of L batsman are higher compared to R of same population. 

I also tested the effect size using  Cohen's d that is determined by calculating the mean difference between your two groups, and then dividing the result by the pooled standard deviation.

Cohen's d = (M2 - M1) divide by  SD

(0.238 - 0.252) divide by  0.033 is 0.424242.

The d value is small and indicates that there is a mean difference between both the groups is small.This maynot have an impact on winning of a game but can impact the individual ranking and grading of the players.

It’s fairly true that in major league baseball left-handed batters , on average, hit better than their right-handed counterparts. 

