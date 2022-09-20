# I310-Assignment-1
# Analyzing the Top 100 Zac Mains for Trends in Personal Statistic Data

# Preface

League of Legends is a MOBA (Multiplayer Online Battle Arena) where teams of 5 players face off against each other with the goal of destroying the enemy 'Nexus'. Recently In-Game, I surpassed the 'Top 500' (Abitrary) milestone on the character (called 'Champions') named Zac. 

# Goal

In this project, I analyze a dataset that I have put together containing the personal statistics of the Top 100 Zac players in the game in order to better understand what stats I need to personally improve upon in order to climb (Rise in Rank) the ranks further. While I do not include my own personal statistics in the framework of this project, I fundamentally believe that an understanding of the information that I present in this project to be of paramount use to anyone wishing to climb at any rank.

# API Documentation

This project utilizes the Pandas and Seaborn Python libraries to build tables and graphs.

Pandas: https://pandas.pydata.org/pandas-docs/stable/reference/index.html
Seaborn: https://seaborn.pydata.org/api.html

# License

MIT License

Copyright (c) 2022 cwolfhope

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

# Source-Of-Data

The dataset for this project was manually compiled from the list of 'Best Zac Players' via the 'Porofessor' Desktop Application. 

The 'Porofessor' Desktop Application can be aquired via the 'Overwolf' app store or viewed with limited access at their webpage: https://porofessor.gg/
Overwolf: https://www.overwolf.com/
An image of this list and an example of the the presentation of this data (using the statistics of the #1 Zac player) can be located at: https://imgur.com/a/t5ltjdo

# Data Types

Within the dataset there is five different types of data that are listed.
These include:
- Rank (Ordered from High to Low)
- Winrate (Describes the winrate of the ranking player's Zac statistics without relation to overall account winrate)
- Average Kills
- Average Deaths
- Average Assists

An additional data type is analyzed within the code pertaining the KDAR (Kill, Death, Assist Ratio; (K+A)/D) of each player

# Sample Bias

As user game data is subject to change rapidly over time, it is highly likely that since collection (Compiled on 9-17-20), the general player statistics of the 'Top 100 Zac Mains' has changed noticeably from the version provided in this project. 

Given the source of the data provided on Porofessor (sourced directly from League of Legends game statistics), it is highly unlikely that the data in the dataset contains bias.

# Analysis

The analysis' in this project observe seven different graphs and take specific notice of the relations between Ranks, Winrates, and other data points to make hypothesis' about the correlations between values in the dataset. The analysis is split into two main scatter plots ranging between scatterplot 1 (graphs 1-2) and scatterplot 2 (graphs 3-7).

Graph #1: 
In graph 1 there is a negative correlation between the rankings (when the values are oriented in a reverse rank value scale; low to high) and winrate that clearly suggests that rank is influenced significantly by winrate. Ranks in League of Legends (LOL) are measured such that the lower in number a rank is, the higher the relative value of the rank(Rank 1 is higher than Rank 100). Additionally, spread of the hue of games played (More games played associated with lower winrate) suggests that the highest ranking Zac players engage in a practice called 'Smurfing'. This occurs when a player creates a new account in order to take advantage of the low amount of games to build player statists that are otherwise irregularily high compared to regular players. While this practice is generally frowned upon in the gaming community, in large games such as LOL, smurfing is almost required in some cercumstances in order to evenly compete with the statistics of other players on the leaderboards.

Graph #2:
Observing graph 2 provides a clearer example of the correlation between higher winrates and a higher relative rank. If a winrate is higher, the player is more likely to be ranked higher as well.

Graph #3:
In graph 3, the spread of the data points is much more centralized as compared to the first scatterplot of graphs 1 and 2. There is of an observable pattern (linear) to the data points (lower ranks-dark hues- lie close to the origin while higher ranks-lighter hues- begin to increase in frequency the farther away from the origin the data point is) that suggests that higher ranks are correlated with higher Kill, Death, Assist Ratios (KDAR/KDA). This matches the observations about correlations made in the previous scatterplot (Winrate correlates with Rank). Based on these observations winrate appears to correlate with KDAR; however, it is unclear which component of KDA plays the biggest role in deciding winrate.

Graph #4:
There is little happening in graph 4. It is the same scatterplot as graph 3, however the hues of the data points are very close to one another (aside from a few outliers that don't describe the shape of the overall dataset) in color which suggests that the Average Kills may not play as big of a role as compare to other values in the dataset.

Graph #5:
A similar story seems to be told by graph 5 as graph 4. There is a seemingly non-correlative parttern to the hues of the dataset(albeit graph 5 seems more random), which suggests that like Average Kills, Average Assists are not the greatest contributor to the highest KDAR values. While it appears there might be less high assist valued hues located close to the origin (which makes logical sense given that those values would be associated with lower KDAR scores), Average Assist values do account for a larger percentage of KDAR scores (formula-wise) in the dataset as compared to Average Kill values which suggests that Assists overall are more important than Kills in matches.

Graph #6:
This graph in particular displays the clearest observable correlation between KDAR and winrate out of all of the variants of the second scatterplot graph. There is a high density of low valued data points (low winrate and KDAR) that are associated with a high number of average deaths. As the graph continues, the hues of the datapoints become lighter in direct correlation with higher KDAR scores. Graph 6 out of all of the graphs seems to indicate that the biggest predictor of high winrate (and thusly a higher likelyhood of high relatively scored rank) is low Average Deaths.

Graph #7:
Recapping some of the analysis' that were made in graphs 3 to 6, graph 7 shows the linear regression of the scatterplot, which as previously predicted shows that higher winrates are directly correlated with high KDAR scores.

# Conclusions

High rankings (lower valued rankings are relatively higher on the leaderboards) are associated with high winrates and low average deaths. Additionally, the analysis of the graphs suggests that keeping deaths low at the expense of kills and assists, is the best way of climbing in rank. Lastly, based on the overall low amount of games played by the majority of highest ranked players, "Smurfing" may be required to actively compete with other players for ranking on the leaderboard.
