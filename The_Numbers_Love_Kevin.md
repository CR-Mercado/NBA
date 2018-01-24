---
title: "The Numbers Love, Kevin"
author: "crmercado"
date: "January 23, 2018"
output: 
  html_document: 
    keep_md: yes
---

# The Statistical Analysis of Kevin Love 

Kevin Love is catching heat online for no reason, as usual. He falls on his sword, in silence, whenever the Cavs go on a losing streak. 

So to remind everyone not just what Kevin Love gave up to be on the Cavaliers, but also to give the K-lovers some ammo against those who support the war on kevin (JR Smith & sponsors) I've done a statistical analysis on all the small things having Kevin Love does for the Cavaliers. 

YES! I know a true analysis would simulate for Kevin Love's replacement, not just analyze games with and without him, but that's not the point! 

#### The Data 

I went to basketball reference and copy pasted Kevin Love's 4 seasons with the Cavaliers into a csv file. It's on github. I cleaned the data by renaming the columns, making missed games "NA" and splitting results into "Result", "PointDifferential" instead of "W (+3)" it's "W" in one and "+3" in another.





### Kevin Love Adds Consistency 

Let's compare apples to apples. Kevin Love has missed games against 21/29 teams in the NBA while on the Cavs. Let's make it fair and only compare Cavs games against those 21 teams for comparison. 

In the 35 games Kevin love's missed in the last 4 seasons the Cavs, here's how the Cavs did with and without him: 


![](The_Numbers_Love_Kevin_files/figure-html/unnamed-chunk-2-1.png)<!-- -->

Look at that giant hole around 0. The blowout nature of loveless games are obvious. Only 2/35 games without Love were decided by less than 5 points compared to 41/186 of games against the same teams with him. A simple t.test shows: this is statistically significant to the .001 level. 


```
## 
## 	Welch Two Sample t-test
## 
## data:  NoLoveCloseGames and YesLoveCloseGames
## t = -3.257, df = 80.461, p-value = 0.00165
## alternative hypothesis: true difference in means is not equal to 0
## 95 percent confidence interval:
##  -0.26304999 -0.06352451
## sample estimates:
##  mean of x  mean of y 
## 0.05714286 0.22043011
```

### Kevin Love is Holding Back to be a Team Player

Let's look at the same concept from two angles. 
How many shots does he take on average in WINS vs Losses. 
Does him taking more shots (than average) correlate well with increasing wins and decreasing losses (i.e. increasing the Point Differential)

Below is a simple plot of his field goal attempts in wins and losses. Notice the small blue and red lines between his average and 18. Kevin Love could safely be averaging up to 18 field goal attempts again with almost no effect on the resulting point differential in wins or losses. 

He's giving up his own stats -Not to improve the Team's results (negligible effect) but to keep others involved.

![](The_Numbers_Love_Kevin_files/figure-html/unnamed-chunk-4-1.png)<!-- -->

### Kevin Love is still Improving 

Don't get too tunnel-visioned over the raw BPM - that's not adjusted for anything. Notice that the relationship between his FG% and his BPM is getting increasingly positive in both wins and losses. 


![](The_Numbers_Love_Kevin_files/figure-html/unnamed-chunk-5-1.png)<!-- -->

Shooting accurately is great, but it's irrelevant if they're scoring just as much. At high FG% he's doing better at converting his score into actual Point Differential. This is of course partly because he's playing with Lebron and getting fully comfortable with the playstyle, but part of it is defense. We're seeing hints of a two-way Kevin Love here.  

### Conclusion

Kevin Love is good at basketball. 

