# Everything you want to know about the 2022 CFB season

What is not to love about college football? 131 teams playing games every Saturday can turn into utter chaos at a moment’s notice. From watching ESPN's college gameday pregame show Saturday mornings to the legendary Pac-12 after dark game, I can’t think of many better ways to spend a Saturday in the fall. 

As part of my data career jumpstart program I decided to visualize a number of metrics from the 2022 college football season using Tableau. The data I used can be found on [kaggle](https://www.kaggle.com/datasets/jeffgallini/college-football-team-stats-2019/code), and also on the NCAA’s website: <https://www.ncaa.com/stats/football/fbs>.

There are ~ 150 metrics (columns) being tracked for the 131 FBS schools, ranging the gamut from offensive yards to defensive 4th down percentage to net turnovers per game and everything in between. There are a seemingly endless number of relationships I could have compared, but I tried to keep my initial analysis pretty simple, mostly looking at offensive and defensive efficiency. 

## Which conference and teams had the most success? ##

<img src="images/conference_wins.png?raw=true"/> (chart showing the number of wins by conference)

In the column chart above I start by plotting each team's wins, color coated by conference. It should come as no surprise to anyone that watches college football that the SEC leads the country in average wins with just over 8. The conference has been dominant over the past decade and a half winning 6 of the last 8, and 13 of the last 17 national championships. It also doesn't hurt that the SEC has an 8 game conference scchedule and each team gets to pad its records with an extra G5 or FCS game.

In addition to wins per team, the table on the bottom left shows a summary of statistics including average offensive and defensive rank. The once great defenses of the SEC are no more, it is actually the Big Ten, led by Iowa, Illinois, and Michigan, that has the strongest conference defensively. Additionally, the Big 12 led by Oklahoma, Texas Tech, and TCU that boasts the strongest conference offensively.

Lastly, on an individual team level there were 13 teams that won 11 or more games this past year. 

## Where do teams stack up offensive and defensively? ##

<img src="images/CFBscatter.png?raw=true"/> (Scatterplot showing offensive and defensive efficiency)

The scatterplot above shows a team’s defensive rank along the x-axis and offensive rank along the y-axis. The top teams in the country find themselves in the bottom left corner, no surprise to see Georgia as the team with the highest combination of offensive and defensive rank. Teams in the top right were among the worst teams in the country, and Colorado tops that list with FIU and Indiana not far behind. Team’s in the bottom right have high powered offense with putrid defense, and teams in the top left play lock down defense, but can’t score the ball. 

In the two tables on the right I also show which team’s defenses most out rank their offense (defensive tilt) and vice versa (offensive tilt). It should come as no surprise that Iowa has the most defensive minded team, with a ranking of 2 and 130 (out of 131). On the offensive side of the ball, it's Georgia Southern with the 18th ranked offense and 129th ranked defense that is most offensively tilted

My main takeaways from this this scatterplot are:
### 1 Georgia really was head and shoulders above the rest of the country ###
On January 9th, 2023 Georgia won their second consecutive national championship. Georgia followed that up in April at the NFL Draft with a leading 10 players drafted. For the seond year in a row Georgia was the class of college football. Many people think Georgia's defense carried the team, while this might have been true in 2021, Georgia's 2022 dominance could be seen on both sides of the ball and the offense even slightly outpaced the defense. Ranking 5th on offense and 10th on defense, Georgia was the only team in the country to be top 10 in both offense and defense, and one of seven teams to be in the top 30 on both sides of the ball.
### 2. Never change Iowa ###
Iowa plays a very ~~niche~~ boring style of football, and year in and year out consistently has one of the top defenses in the country. This year was no exception, with Iowa's defense ranking number 2 in the nation. The offense on the other hand was an embarrassment ranking 130 out of 131 teams. The team’s defensive tilt score of 128 is only two points away from the highest possible value. The offense was so dysfunctional that a stipulation for the 2023 season was included in offensive coordinator Brian Ferentz’ contract requiring the team to score 25 points a game in order for him to keep his job. Midway through the 2023 season, it does not appear Iowa, currently averaging 19.5 points per game, will reach that target.
### 3. Lincoln Riley might have gone west, but Oklahoma hasn’t realized it yet ###
Lincoln Riley was the head coach at Oklahoma for five years and during his tenure the Sooners were known for a high powered offense and a lackluster defense. During his Oklahoma tenure, he coached two Heisman winning quarterbacks and another NFL starter. The team always had a top ranked but couldn't figure it out on the defensive side of the ball to be a true national title contender. Fast forward to 2022 and Lincoln Riley is now at USC, coaching another Heisman winning quarterback in Caleb Williams, and similar to his time at Oklahoma, the Trojans defense let down the team at the end of last year. In terms of offense rank number 5 in offensive tilt, but Riley’s old school, Oklahoma, ranks number 3.
### 4 Colorado was in really really bad shape ###
Much has been made in the early part of this year’s college football season about Deion Sanders' turnaround of the Colorado Buffalo program. Coach Prime has already led Colorado to 4 wins, greatly exceeding their expectations for the year. Colorado was one of the worst teams in 2022, going 1-11, but just how bad were the Buffalo last year?. Colorado was bottom 4 on the offensive and defensive side of the ball. A truly stunning feat for a power 5 conference team. 

## Who were the most complete teams in the Country? ##

<img src="images/juggernauts.png?raw=true"/> (juggernauts - team ranking top 30 on both offense and defense)

As I mentioned before, Georgia was the only team to finish top 10 on both sides of the ball. Overall, 7 teams finished the season in both the top 30 offense and defenses: Georgia, Ohio St, Alabama, Florida St, Michigan,Utah, and newly promoted FBS school Jame Madison. Three of these teams: Georgia, Michigan, and Ohio St, made the college football playoff; three more: Alabama, Florida St, and Utah, won double digit games. The unexpected team in this category was the James Madison Dukes, who in their first year as an FBS school dominated the early part of the Sun Belt season before faltering down the stretch.
