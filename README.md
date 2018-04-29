   
Visualization for Peers
===========
# Jonishuxi Final Project
* ## Joshua Allen
* ## Shuihui Tang
* ## Xingxing Zhang
* ## Nihali Jain
### Data Vis IS590

The data set is named Lahman’s Baseball Database and it can be find in seanlahman.com. The URL is http://seanlahman.com/baseball-archive/statistics/

The database contains complete batting and pitching statistics from 1871 to 2018, plus fielding statistics, standings, team stats, managerial records, post-season data, FieldingOFsplit, Parks, HomeGames, and more.It includes data from the two current leagues (American and National), the four other "major" leagues (American Association, Union Association, Players League, and Federal League), and the National Association of 1871-1875. The database can be used on any platform, but please be aware that this is not a standalone application. It is a database that requires Microsoft Access or some other relational database software to be useful.

The database has 28 csv files and most of them have more than 5000 records and the biggest one has more than a hundred thousand rocords.

### Limited Use License
This database is copyright 1996-2018 by Sean Lahman.

This work is licensed under a Creative Commons Attribution-ShareAlike 3.0 Unported License.  For details see: http://creativecommons.org/licenses/by-sa/3.0/

Thanks to Ted Turocy of the Chadwick Baseball Bureau, who did the heavy lifting to make the 2016 update possible. Ted also hosts a version of the data at github, for folks who are inclined to interface with it that way. Mike Webb created the SQL version.

## Salary by position across the years

This plot shows the range of salaries at each position at different year. We can use the slider to choose which year you want to looking at. Also, when you move to each bar, it can show the exact salary. We are curious about which position can make the most money in a baseball game. So we combined "salary" and "fielding" these two datasets together in one dataframe called "player_position." Because we already explored these two datasets and found out that they both have "playerID" and "yearID," then we merged them and created a new dataset with only four colums.

Initially, we showed the data as a line graph for each position across the years. This plot shows all the positions as a bar graph for a given year. Sliding through the years gives a more visual contrast to how the pay rates have changed.


<a name="figure"></a>
    
<div class="bk-root">
    <div class="bk-plotdiv" id="53026025-0272-44bc-abc9-06d7a7cc4cd3"></div>
</div>
