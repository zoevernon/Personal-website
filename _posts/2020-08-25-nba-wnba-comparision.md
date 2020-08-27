---
title: 'Comparing the NBA and WNBA'
date: 2020-08-10
permalink: /posts/2020/08/nba-wnba-comparison/
---

Do you like the offensive rebounding? How about the midrange game? Are you a fan of the Rockets? Or wish you could watch the 2014-15 Warriors again? Well, I'm here to tell you that you might enjoy watching the WNBA and  help find your potential new favorite team! 

In addition to matching NBA teams with comparable teams in the WNBA I compare the leagues in a number of statistics throughout the last 10 seasons.   To address these questions I created a Shiny app hosted [**here**](https://zoevernon.shinyapps.io/nba_wnba_comparison/).  In the app you can compare any team from 2010-2020 in both the NBA and WNBA for a number of different statistical categories as well as see the change over time in each league.  

I present some of the interesting obseravations I found from using the app in this post, but encourage you to play with it on your own!  


## Differences between the leagues 
First, I wanted to figure out how the WNBA differs from the NBA across the last 10 seasons.  The two leagues have largely followed similar trajectories (i.e. more threes and less offensive rebounds) but there are many differences between them, some surprising and others more obvious. 

After watching a couple WNBA games one of the most apparent distinctions is the shot distribution.  Most WNBA teams seem to take far more midrange shots than is customary in the present day NBA, and that is exactly what we see in the data.  Given that WNBA games are shorter than the NBA we compare the shot distributions between the two leagues by looking at the number of shot attempts from a given location per possession.  This allows us to look at differences without needing to adjust for time or pace.  

Using data from [stats.nba.com](stats.nba.com) and [stats.wnba.com](stats.wnba.com), we see in the figure below that every WNBA team in the 2020 season take more midrange shots (5 - 19 feet) than the average NBA team in the 2019-20 season.  The New York Liberty take by far the least in the mid range while the Las Vegas Aces, with A'ja Wilson and their interior dominance, take over 0.4 shots per possession from these distances.  In the NBA San Antonio are the only team that take more than 0.3 shots per possession of their shots from 5 - 19 feet, and the Houston Rockets take only 0.15.  

![Midrange distributions](/figures/midrange_dist.png)
Note, an interactive version of this plot where you can see where all teams fall on the distribution is in the Shinny app.  For purposes of formatting I made a static version for this post.  
 <!---<iframe width="800" height="500" frameborder="0" scrolling="no" src="//plotly.com/~zo3v3rnon/1.embed"></iframe>--->

In addition to looking at how the distributions differ between teams this season, I looked at the change over the last 10 seasons.  Here we see that the reduction in midrange shots has occurred much more dramatically in the NBA than the WNBA.  

 <!---<iframe width="800" height="500" frameborder="0" scrolling="no" src="//plotly.com/~zo3v3rnon/3.embed"></iframe>--->
![Midrange by year](/figures/midrange_by_year.png)

This increase in midrange shot taking is coupled with less shot attempts, in the WNBA, from three point range.  Below, we see the trend in 3 point attempts per possession over time.   To see the distribution for the 2020 WNBA and 2019-20 NBA seasons check [Shiny app](https://zoevernon.shinyapps.io/nba_wnba_comparison/).    Prior to moving the three point line back for the 2013 season, WNBA teams were taking more 3FGA per possession than NBA team on average, but over the last decade the increase in three point attempts in the NBA has been much more dramatic.    
 
 ![Three pointers](/figures/three_attempted_by_year.png)
 <!--- <iframe width="800" height="500" frameborder="0" scrolling="no" src="//plotly.com/~zo3v3rnon/5.embed"></iframe> --->
 <!---<iframe width="800" height="500" frameborder="0" scrolling="no" src="//plotly.com/~zo3v3rnon/7.embed"></iframe>--->

There are a number of other statistics which differ between the leagues including, FG % (higher in the NBA), FT % (higher in the WNBA), offensive rebound % (higher in the WNBA), and pace (higher in the NBA).  I encourage you to explore the season by season distributions and overall trends of those statistics.  

 <!--- At this point the obvious question to ask is why is this the case?  Is the WNBA less sold on analytics, which has shown the superiority of the three pointer?  Or is there a fundamental difference between the leagues that makes threes less valuable in the WNBA?  --->

 <!--- Without knowing the extent to which WNBA teams have analytics departments, I think the answer is falls somewhere in between.  Looking at the difference in 3FG % between the two leagues we can see that WNBA players shoot much worse than NBA players from 3, however, they also shoot worse from 2.  It seems that only --->

 <!--- Across the board NBA players, shoot a higher percentage from the field.   However, WNBA players are much better FT shooters.   When it comes to 3 pointers we can see the impact of the extension of the 3 point line in the WNBA before the 2013 season.    Prior to the change, the WNBA was not only shooting more threes than NBA teams at the time, but they were shooting better from three.  Over time WNBA players have adjusted and despite, a slower increase in 3 pointers per possession, they have dramatically increased 3 point percentage over the last couple years.  --->

<!---  <iframe width="800" height="500" frameborder="0" scrolling="no" src="//plotly.com/~zo3v3rnon/13.embed"></iframe>  --->

<!--- <iframe width="800" height="500" frameborder="0" scrolling="no" src="//plotly.com/~zo3v3rnon/11.embed"></iframe>  --->

<!--- <iframe width="800" height="500" frameborder="0" scrolling="no" src="//plotly.com/~zo3v3rnon/9.embed"></iframe>  --->

<!--- <iframe width="800" height="500" frameborder="0" scrolling="no" src="//plotly.com/~zo3v3rnon/15.embed"></iframe>  --->

## Which WNBA team should I root for?
The [app](https://zoevernon.shinyapps.io/nba_wnba_comparison/) can help you find the best fit in the WNBA based on the statistics that you care about for your favorite NBA team.  Note, that as we see above the leagues are quite different, so although comparing them is not perfect it's still a fun!   Below are a couple examples.  

### The Milwaukee Bucks
Let's say I want to see which WNBA teams play most like the Bucks across all the statistical categories we have available.   Then we would see that the Chicago Sky are most similar, followed by the Las Vegas Aces and the Seattle Storm.   In general, the better WNBA teams are more similar to the Bucks and the worse teams are less similar.   

![Bucks comparision](/figures/bucks_all.png)

### The Houston Rockets
If your favorite thing to do is watch an offense predicated around the three pointer, you could see which WNBA teams are most like the Rockets in terms of their shot distribution (by selecting FGA from various distances).  In that case you may want to tune into the New York Liberty or the Connecticut Sun, but definitely not the Aces.  

![Rockets comparision](/figures/rockets_fga.png)

However, be warned about the Liberty, because although they take a lot of threes, they don't shoot a high percentage.  In fact, if we include FG% statistics in addition to the FGA stats, we see that the Liberty are one of the similar teams to the Rockets... try that for yourself in the app if you want to see the change.  

### The 2014-15 Warriors
As a final example, let's say that you just loved watching the Warriors offense on the way to the first title in their recent run, because I mean who didn't? In that case tune in the Storm, Sky, or Sparks.  

![Warriors comparision](/figures/warriors_off.png)

