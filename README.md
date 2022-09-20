# I310-Assignment-1
# Analyzing the Top 100 Zac Mains for Trends in Personal Statistic Data

# Preface
League of Legends is a MOBA (Multiplayer Online Battle Arena) where teams of 5 players face off against each other with the goal of destroying the enemy 'Nexus'. Recently In-Game, I surpassed the 'Top 500' (Abitrary) milestone on the character (called 'Legends') named Zac. 

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
