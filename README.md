<header>
<link rel="stylesheet" href="http://cdn.pydata.org/bokeh/release/bokeh-0.11.1.min.css" type="text/css" />
<script type="text/javascript" src="http://cdn.pydata.org/bokeh/release/bokeh-0.11.1.min.js"></script>
<script type="text/javascript">
(function() {
     var fn = function() {
       Bokeh.safely(function() {
         (function(root) {
           function embed_document(root) {
             
           var docs_json = '{"88c57a72-d03c-48b6-9b92-bdaff104d387":{"roots":{"references":[{"attributes":{"callback":null,"tooltips":[["Position: ","@pos"],["Salary: ","$y{(0,0)}"]]},"id":"72dbc6a5-ee7e-4cef-b353-8ba68bcfbdea","type":"HoverTool"},{"attributes":{},"id":"b959a836-c310-4e6f-a865-964de4c86d0e","type":"LinearScale"},{"attributes":{"axis_label":"Salary","formatter":{"id":"9a69664c-d33e-42b8-840d-034ab4bc5f55","type":"NumeralTickFormatter"},"plot":{"id":"928e3750-4536-41de-99ca-4d7f7add34d6","subtype":"Figure","type":"Plot"},"ticker":{"id":"33941359-1c9d-4f4e-a54d-fa61a445152f","type":"BasicTicker"}},"id":"9ec06bb6-4caa-44ed-ad00-aa23d8654333","type":"LinearAxis"},{"attributes":{},"id":"ff0e003e-88b6-4294-aa1b-5e54535024d5","type":"CategoricalTickFormatter"},{"attributes":{"source":{"id":"1fa7ad41-115f-42f8-a7c1-bfb01315b423","type":"ColumnDataSource"}},"id":"c74b2ae9-0815-4b57-a4a9-b3e92cf69cfb","type":"CDSView"},{"attributes":{"fill_color":{"field":"color"},"line_color":{"field":"color"},"top":{"field":"salary"},"width":{"value":0.9},"x":{"field":"pos"}},"id":"dcb9ad86-7c75-4a7c-83a6-3840b6575d74","type":"VBar"},{"attributes":{"data_source":{"id":"1fa7ad41-115f-42f8-a7c1-bfb01315b423","type":"ColumnDataSource"},"glyph":{"id":"dcb9ad86-7c75-4a7c-83a6-3840b6575d74","type":"VBar"},"hover_glyph":null,"muted_glyph":null,"nonselection_glyph":{"id":"aec8155a-b597-4c81-ae35-94910c6867c5","type":"VBar"},"selection_glyph":null,"view":{"id":"c74b2ae9-0815-4b57-a4a9-b3e92cf69cfb","type":"CDSView"}},"id":"97bb0cb2-996a-4378-a11f-093f8780b383","type":"GlyphRenderer"},{"attributes":{"plot":null,"text":"Salaries in different positions"},"id":"924045b5-abf2-4062-a25f-32ff5f52b360","type":"Title"},{"attributes":{"active_drag":"auto","active_inspect":"auto","active_scroll":"auto","active_tap":"auto","tools":[{"id":"72dbc6a5-ee7e-4cef-b353-8ba68bcfbdea","type":"HoverTool"}]},"id":"026217e9-2822-4dad-8f34-7f1d3a97ce67","type":"Toolbar"},{"attributes":{"axis_label":"Position","formatter":{"id":"ff0e003e-88b6-4294-aa1b-5e54535024d5","type":"CategoricalTickFormatter"},"plot":{"id":"928e3750-4536-41de-99ca-4d7f7add34d6","subtype":"Figure","type":"Plot"},"ticker":{"id":"9b35e1ba-9605-4a04-b94b-38e9e2ccaed8","type":"CategoricalTicker"}},"id":"05fb6314-0313-4774-a8b8-437b130d4578","type":"CategoricalAxis"},{"attributes":{"callback":null,"factors":["1B","2B","3B","C","OF","P","SS"]},"id":"b3ddf119-a89c-44e4-ab8f-ba89f1b15597","type":"FactorRange"},{"attributes":{"plot":{"id":"928e3750-4536-41de-99ca-4d7f7add34d6","subtype":"Figure","type":"Plot"},"ticker":{"id":"9b35e1ba-9605-4a04-b94b-38e9e2ccaed8","type":"CategoricalTicker"}},"id":"546d84ec-3a81-4c75-9ffd-d075eb13d40b","type":"Grid"},{"attributes":{},"id":"17239136-6c61-4773-8147-33516601e43a","type":"CategoricalScale"},{"attributes":{},"id":"9b35e1ba-9605-4a04-b94b-38e9e2ccaed8","type":"CategoricalTicker"},{"attributes":{"dimension":1,"plot":{"id":"928e3750-4536-41de-99ca-4d7f7add34d6","subtype":"Figure","type":"Plot"},"ticker":{"id":"33941359-1c9d-4f4e-a54d-fa61a445152f","type":"BasicTicker"}},"id":"ad64d1ab-09df-4f29-9199-d5f1693acea3","type":"Grid"},{"attributes":{"callback":null,"column_names":["pos","salary","color"],"data":{"color":["#440154","#443982","#30678D","#208F8C","#35B778","#8DD644","#FDE724"],"pos":["1B","2B","3B","C","OF","P","SS"],"salary":[11166667,7196656,8500000,12071429,12868670,15714286,10000000]},"selected":null,"selection_policy":null},"id":"1fa7ad41-115f-42f8-a7c1-bfb01315b423","type":"ColumnDataSource"},{"attributes":{"items":[{"id":"f685c8eb-8aea-4c79-9624-c832797ff815","type":"LegendItem"}],"orientation":"horizontal","plot":{"id":"928e3750-4536-41de-99ca-4d7f7add34d6","subtype":"Figure","type":"Plot"}},"id":"cbd5f8f3-8cdb-453b-8421-7d9cef80effb","type":"Legend"},{"attributes":{},"id":"33941359-1c9d-4f4e-a54d-fa61a445152f","type":"BasicTicker"},{"attributes":{"fill_alpha":{"value":0.1},"fill_color":{"value":"#1f77b4"},"line_alpha":{"value":0.1},"line_color":{"value":"#1f77b4"},"top":{"field":"salary"},"width":{"value":0.9},"x":{"field":"pos"}},"id":"aec8155a-b597-4c81-ae35-94910c6867c5","type":"VBar"},{"attributes":{"label":{"field":"pos"},"renderers":[{"id":"97bb0cb2-996a-4378-a11f-093f8780b383","type":"GlyphRenderer"}]},"id":"f685c8eb-8aea-4c79-9624-c832797ff815","type":"LegendItem"},{"attributes":{"below":[{"id":"05fb6314-0313-4774-a8b8-437b130d4578","type":"CategoricalAxis"}],"left":[{"id":"9ec06bb6-4caa-44ed-ad00-aa23d8654333","type":"LinearAxis"}],"renderers":[{"id":"05fb6314-0313-4774-a8b8-437b130d4578","type":"CategoricalAxis"},{"id":"546d84ec-3a81-4c75-9ffd-d075eb13d40b","type":"Grid"},{"id":"9ec06bb6-4caa-44ed-ad00-aa23d8654333","type":"LinearAxis"},{"id":"ad64d1ab-09df-4f29-9199-d5f1693acea3","type":"Grid"},{"id":"cbd5f8f3-8cdb-453b-8421-7d9cef80effb","type":"Legend"},{"id":"97bb0cb2-996a-4378-a11f-093f8780b383","type":"GlyphRenderer"}],"title":{"id":"924045b5-abf2-4062-a25f-32ff5f52b360","type":"Title"},"toolbar":{"id":"026217e9-2822-4dad-8f34-7f1d3a97ce67","type":"Toolbar"},"x_range":{"id":"b3ddf119-a89c-44e4-ab8f-ba89f1b15597","type":"FactorRange"},"x_scale":{"id":"17239136-6c61-4773-8147-33516601e43a","type":"CategoricalScale"},"y_range":{"id":"4dea1ebb-7baf-4736-97b5-b560fa8640c8","type":"DataRange1d"},"y_scale":{"id":"b959a836-c310-4e6f-a865-964de4c86d0e","type":"LinearScale"}},"id":"928e3750-4536-41de-99ca-4d7f7add34d6","subtype":"Figure","type":"Plot"},{"attributes":{"format":"$0,0"},"id":"9a69664c-d33e-42b8-840d-034ab4bc5f55","type":"NumeralTickFormatter"},{"attributes":{"callback":null},"id":"4dea1ebb-7baf-4736-97b5-b560fa8640c8","type":"DataRange1d"}],"root_ids":["928e3750-4536-41de-99ca-4d7f7add34d6"]},"title":"Bokeh Application","version":"0.12.15"}}';
           var render_items = [{"docid":"88c57a72-d03c-48b6-9b92-bdaff104d387","elementid":"53026025-0272-44bc-abc9-06d7a7cc4cd3","modelid":"928e3750-4536-41de-99ca-4d7f7add34d6"}];
           root.Bokeh.embed.embed_items(docs_json, render_items);
         
           }
           if (root.Bokeh !== undefined) {
             embed_document(root);
           } else {
             var attempts = 0;
             var timer = setInterval(function(root) {
               if (root.Bokeh !== undefined) {
                 embed_document(root);
                 clearInterval(timer);
               }
               attempts++;
               if (attempts > 100) {
                 console.log("Bokeh: ERROR: Unable to run BokehJS code because BokehJS library is missing")
                 clearInterval(timer);
               }
             }, 10, root)
           }
         })(window);
       });
     };
     if (document.readyState != "loading") fn();
     else document.addEventListener("DOMContentLoaded", fn);
   })();
 </script>
 </header>

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
