
[Back to home page](/README.md)

## Visualizing Government Debt Using Tableau

Here we used the publicly available Debt-Y Ratio data (https://data.oecd.org/).  
(Data Source: “General Government - General Government Debt - OECD Data.” theOECD, http://data.oecd.org/gga/general-government-debt.htm. Accessed 28 Jan. 2024) 

This data has government debt by country for 1995 - 2021.

We analyze the data using 3 different visualizations:

## 1. OECD Website Visulization
<iframe src="https://data.oecd.org/chart/7klH" width="860" height="645" style="border: 0" mozallowfullscreen="true" webkitallowfullscreen="true" allowfullscreen="true"><a href="https://data.oecd.org/chart/7klH" target="_blank">OECD Chart: General government debt, Total, % of GDP, Annual, 2020</a></iframe>


The first visual analyzes the metric for 2020 across countries and also how it compares to OECD average. Placed in an ascending order, countries to the right of this marker (OECD Average) have high debt-Y ratio compared to OECD average and vice-versa.


## 2. Vizualizing Same Data on Tableau
<div class='tableauPlaceholder' id='viz1706492282954' style='position: relative'><noscript><a href='#'><img alt='HeatMap: GDP-Y Ratio OECD Countries“General Government - General Government Debt - OECD Data.” theOECD, http:&#47;&#47;data.oecd.org&#47;gga&#47;general-government-debt.htm. Accessed 28 Jan. 2024.  ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;TB&#47;TB_wkb&#47;HeatMapGDP-YRatioOECD&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='TB_wkb&#47;HeatMapGDP-YRatioOECD' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;TB&#47;TB_wkb&#47;HeatMapGDP-YRatioOECD&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='en-US' /></object></div>

<script type='text/javascript'>  
  var divElement = document.getElementById('viz1706492282954');  
  var vizElement = divElement.getElementsByTagName('object')[0]; 
  vizElement.style.width='100%';vizElement.style.height=(divElement.offsetWidth*0.75)+'px'; 
  var scriptElement = document.createElement('script'); 
  scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js'; 
  vizElement.parentNode.insertBefore(scriptElement, vizElement);
</script>


The heat-map presents a comprehensive view of the Debt-GDP ratio's movement across countries over the years. The color scale makes tracking easy for each country: blue to orange shows country moving from a good state to bad state and vice versa.
 
## 3. Tableau Vizualization Considering European Countries Only
<div class='tableauPlaceholder' id='viz1706492216762' style='position: relative'><noscript><a href='#'><img alt='Last 5 Years Average Debt-Y Ratio: European Countries2015-2019 Average: Some countries in the continent are doing well, while others are spiralling into dangerous zones. Task ahead for the Euro Zone ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;TB&#47;TB_wkb_part3&#47;Part32&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='TB_wkb_part3&#47;Part32' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;TB&#47;TB_wkb_part3&#47;Part32&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='en-US' /><param name='filter' value='publish=yes' /></object></div>                
<script type='text/javascript'>
  var divElement = document.getElementById('viz1706492216762');
  var vizElement = divElement.getElementsByTagName('object')[0];
  vizElement.style.width='100%';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';
  var scriptElement = document.createElement('script');  
  scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js'; 
  vizElement.parentNode.insertBefore(scriptElement, vizElement); 
</script>


The third visual considers last 5 years' average for only European countries to help EU leaders identify and focus on countries overdrawing (in red).

Comparing the 3 visuals:
1. The first visual would be relevant in the annual OECD country meet. It clearly shows countries that are doing worse than OECD average. A color scale variation (blue-red for good-worse) could have been useful but the current graph conveys the same information without adding color-noise. If the presenter wanted audience to focus on specific countries (like say Japan, Italy, Greece - that are doing worst), highlighting only these and others in grey would have been useful.
2. The heatmap is useful to analyse year-year movement and also identify countries that might be starting on a spiral. The easy and intuitive color variation (blue for cool/non-dangerous values, and red for alarming/dangerous values of the debt-metric) can also help identify countries that got out of debt; Japan, Greece can learn from the steps taken by these countries.
3. The third visual was created for EU leaders only. Bar chart with intuitive color scale (blue for cool, and red for those requiring attention) was chosen to draw attention to countries that need focus. While reading the number from x-axis requires some eye tracing, but the vertical grid-lines together with the color scale convey the story just as easily, without making the chart text heavy. I wanted the focus more to be on the difference in debt levels within the continent, than on the value of the metric.

Each of the 3 visuals serve a different audience and purpose. While the first one gives a comprehensive view of all OECD countries, the second would be useful to analyze movement over the years. The third would be relevant for EU discussions. While the first gives reader the freedom to read take away what they want (the only marker being the OECD average) - some may focus on the countries with highest debt, others might want to look at how OECD group is doing okay overall; the second and third visuals with their color variation guide and aid the reader in analyzing patters,
