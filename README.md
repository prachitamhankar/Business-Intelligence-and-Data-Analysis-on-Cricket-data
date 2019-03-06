# Business-Intelligence-and-Data-Analysis-on-Cricket-data
Business Intelligence and Data Warehousing using ETL tool Pentaho

## Motivation & Background about Indian Premier League:

IPL is a Cricket tournament played in India which has various franchise-based teams which compete against each other to emerge as a winner. In this twenty over tournament, first toss takes place to decide which team will bat first and which team will bat second. There are two teams with eleven players in the side and these eleven players are a mix of Batsmen, Bowlers, Wicket Keeper and All-rounder. Each team bats for the twenty overs in an innings, every over there are six legal balls that are bowled by the bowling team and the batting team tries to score the maximum runs in the innings and sets a target for the other team. Once the batting team finishes its innings the team that bowled starts to bat for twenty over and tries to chase its target set by the team batting first, if the team chases the target within the twenty overs it emerges as the winner but if the team is not able to chase the set target, the team that batted first wins the match.

## Business Scenario:
The franchise team owners face challenges in identifying the players performance, Price of the match tickets at each stadium that generate revenue for the franchise, which players to retain and which not to and Analysis of Toss Results of each stadium.

## Business Processes:
1) **Descriptive Analysis of Player Performance-** For the batsman, calculation is done for total number of runs scored and their strike rate over the seasons. For the bowlers, calculation is total number of wickets taken and their average over the seasons and for the season’s user want to view. This would make easier for the team owners to choose players from the entire list they want to keep in their teams. 
2) **Predictive Analysis of Price for Auction of Players-** Different franchises bid for different players to form a strong and desirable team that can win the tournament for them. The starting auction amount of each player is decided by the player itself and then based on the highest amount spent by franchise, that franchise gets the player into its team. The same auction amount is paid by the franchise to the players at the end of tournament. Prediction has been made on the dashboard whether a player’s price will go up or down based 4 on their total performance and performance over the season. Dashboard for such scenarios help team owner if they want to increase their bet on the same player and try to go for some other player in the auction. 
3) **Prescriptive Analysis for Retention of Players-** Every franchise can retain up to 3 players based on the performance so the franchise owners can set up the criteria such as number of runs and wickets taken to find which players to retain and which not to retain.
4) **Analysis of Toss Results-** Before commencement of the match, toss decides which teams= will bat first.  Toss plays crucial role in the results of the match as the captains can choose based on the pitch conditions and players in the team batting first is their stronger aspect or batting second is aspect. Old toss results will provide an insightful analysis about the stadium on which stadium to bat first and which to bowl first.

![image_descript](/images/1.png)

**Steps taken:**
1) Take input files and load Data from CSV and Excel files into the database. 
2) Designed an ODS database by joining multiple tables and keeping only the essential attributes which were required to create the dimension table and fact table for the Analysis. 
3) Designed a Data Warehouse where the dimension tables were loaded from the ODS database keeping in mind different dimensions and facts for the purpose of analysis. 
4) Created a fact table inside the Warehouse where only facts which were to be shown in Tableau were stored.

## Tableau Dashboards:

1) **Dashboard for Toss Scenario:** Here we have shown the heat map for the stadiums of IPL which indicates on which stadium the teams that have won the toss, have also won the match, this would help the teams to understand what things should be done on which stadium, whether they should bat first or bowl first.

![image_descript](/images/2.png)


2) **Dashboard for prices of match tickets:** The bar chart in the dashboard denotes the average price of a ticket in an IPL season every year. Moreover, this dashboard provides full control to the user to check the prices of different stands at any venue for all the seasons. 

![image_descript](/images/3.png)

3) **Dashboard for Most Expensive Player:** The below bubble chart shows the most expensive buys of IPL auction 2018. It also gives user control to check the most expensive players according to the type of players. For example, user can view top 10 expensive batsman, bowlers, all-rounders and so on. 
![image_descript](/images/4.png)

4) **Dashboard for Player Analysis:** This dashboard provides the player statistics of all seasons. The user can view highest run scorers and wicket takers till now. Also, the user can check the same stats for each season to know the Orange Cap winner (highest runs in a season) and Purple Cap winner. Moreover, the user can view stats for players for each team for all the seasons or any one season. It also displays the average strike rate and average bowling rate for each batsman and bowler respectively. 

![image_descript](/images/5.png)

5) **Batsman/Bowler Retention:** This dashboard is designed for owners who wish to check stats of their players of all the seasons. Before a new season starts, the owners can put some runs criteria he/she wishes to check, and then it shows a list of players with recommendations whether a player should be retained or not based on the filter value entered by the owner/user. 

![image_descript](/images/6.png)

6) **Predictive analysis for upcoming auction:** We created one calculation categorized on price of players in previous seasons. According to their price, the stats criteria is defined, and this dashboard predicts whether a player’s price should increase or remain same in the upcoming auction. 

![image_descript](/images/7.png)

**Key Learnings from the Project**
1) Learnt how to handle high volume and variety of data altogether. 
2) Learnt how to use SQL queries along with the cases inside ETL tool 
3) We found that visualized data provided more insights than data represented in numeric and string form. 
4) Swim Lane diagrams made it easier to understand the process as compared to directly generating the data model diagram for the same.


## Acknowledgments

* [Indian Premier League](https://www.iplt20.com)
* [Wikipedia](https://en.wikipedia.org/wiki/Indian_Premier_League)
* [Data World](www.data.world.com)


