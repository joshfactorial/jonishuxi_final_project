   
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


```python
#from bokeh.plotting import *
#from bokeh.models import HoverTool
from bokeh.embed import components
#import pandas as pd
#from ipywidgets import interact
#import bokeh
from bokeh.io import show, output_file, output_notebook
from bokeh.plotting import figure
from bokeh.palettes import Viridis
from bokeh.models import ColumnDataSource, HoverTool,NumeralTickFormatter
import pandas as pd
#import ipywidgets
from ipywidgets import interact
#import matplotlib.pyplot as plt
#import numpy as np
#from scipy.stats import gaussian_kde

output_notebook()
hover = HoverTool(tooltips=[
   ("Position: ","@pos"),
   ("Salary: ","$y{(0,0)}")
])

salary = pd.read_csv("data/Salaries.csv")
fielding = pd.read_csv("data/Fielding.csv")
player_position = pd.merge(salary, fielding, on = ["playerID","yearID"])[["yearID", "playerID", "salary", "POS"]]
data = player_position.groupby(["yearID", "POS"]).mean()["salary"].unstack()
d = {}
d = {"1B" : 'b-', "2B" : 'c-',"3B" : 'g-',"OF":'g--',"SS":'y-',"P":'r-',"C" :'k-'}

def fi(year):
    x = player_position[player_position["yearID"]==year]
    #print(x)
    data = x.groupby("POS").max()["salary"].reset_index()
    pos=[]
    for i in data["POS"]:
        pos.append(i)
    #print(data["POS"])
    #print(pos)
    sal=[]
    for i in data["salary"]:
        sal.append(i)
    source=ColumnDataSource(data=dict(pos=pos,salary=sal,color=Viridis[7]))
    #sal = data["salary"]
    #print(pos)
    p=figure(x_range=pos,title="Salaries in different positions",tools=[hover])
    p.vbar(x="pos",top="salary",color="color",source=source,legend="pos",width=0.9)
    p.legend.orientation = "horizontal"
    p.xaxis.axis_label = "Position"
    p.yaxis[0].formatter = NumeralTickFormatter(format="$0,0")
    p.yaxis.axis_label = "Salary"
    show(p)
    #print(data)

interact(fi,year=(1985,2016))
```

Test

