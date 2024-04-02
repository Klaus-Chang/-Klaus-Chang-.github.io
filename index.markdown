---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
---
<head>
  <meta name="description" content="{{ Contributor | escape }}">
  <link rel="shortcut icon" type="image/png" href="/assets/img/DTU_Logo_Corporate_Red_RGB.png"/>
</head>
<img src="{{ '/assets/img/DTU_Logo_Corporate_Red_RGB.png' | relative_url }}" alt="Site logo">
<div class="content-section">
  <h1>Deciphering the Data: A Preliminary Look at Crime and Safety in San Francisco</h1>
  <p>In San Francisco, a new research project is exploring the city's crime data to help the public understand the safety of their neighborhoods. The study's dataset is sourced from the official website of SF.gov at <a href="https://data.sfgov.org/">https://data.sfgov.org/</a>, a platform that centralizes data from multiple departments and public agencies with the goal of improving accessibility and efficiency of services while saving taxpayer dollars through the efforts of digital and data services teams.</p>
  <p>The dataset used in the study contains a wealth of column information, including case ID (PdId), Incident number (IncidntNum), incident code (Incident Code), Category, Descript, Day of the week, Date, Time, PdDistrict, Resolution, Address, coordinate X, coordinate Y, and location (location). With this data, researchers can conduct in-depth analyses to identify areas and time periods of high crime rates, as well as trends in specific crime types.</p>
  <p>Using data visualization tools such as Plotly, the researchers were able to map clearly which places are relatively safe and which are likely to require more public attention. This visual approach not only helps the public understand the security situation in the community, but also visually shows the areas where certain types of crime are most common, or when crime incidents are most common.</p>
  <p>In addition, most of the graphic design is designed to visually communicate information, such as by reading the bar chart, the public can quickly learn which types of crime incidents are the most frequent, and by visualizing the map, which areas are relatively safe or dangerous.</p>
  <p>It's worth noting that while the study covered data from 2003 to the end of 2017, the latest data is available from 2018 to the present on SF.gov. For readers interested in such studies, they can download the data directly to conduct their own analysis and research.</p>
  <p>Through the regional and temporal analysis of crime data, this project not only increases public awareness of community safety, but also provides a practical tool that enables people to make more informed decisions based on data, thereby improving their quality of life.</p>
</div>

<div class="content-section">
  <h1>Three visualizations</h1>
  <h2>Ⅰ Number of Crimes per Hour of the Week by Category</h2>
  <img src="assets/img/crimes_per_hour_of_the_week.png" alt="Number of Crimes per Hour of the Week by Category">
  <p>Each crime type shows a pattern of crime distribution over the course of a week, and it can be seen that certain crimes have a distinct high incidence period at certain times.</p>
  <p>The spikes in some charts are higher than others, suggesting that some types of crime are more common than others. The number of burglaries, for example, is significantly higher than cases of drunkenness or drugs.</p>
  <p>Such information could be particularly useful for law enforcement agencies in crime prevention and resource allocation, as it could guide them to step up policing at specific times of the week.</p>
  <p>At the same time, it is also very good information for people living in the nearby communities, and they can make targeted measures based on this information to protect themselves and their families.</p>
  <h2>Ⅱ Visualizing geodata</h2>
  <embed
   type="text/html" 
   src="/assets/map.html" 
   width="800" 
   height="600">
  <p>The colors for many areas can be very similar, making the visual differences less apparent." I try to use a logarithmic scale for color mapping, which would reduce the visual gap between high and low values, making the differences in mid-range values more pronounced. </p>
  <p>As a result, we can clearly see from the graph that parking in the Richmond area on Sundays is the safest, while the Southern area is the least safe for parking.</p>
  <h2>Ⅲ Interactive visualizations</h2>
  <embed
   type="text/html" 
   src="/assets/Interactive_visualization_small.html" 
   width="1000" 
   height="1000">
  <p>Unfortunately, if we want to fully replicate the effect of clicking on the legend to hide data on this scatter plot, the overall size of the webpage would become very large, and the browsing speed would be very slow—even with a limited amount of data. Therefore, in order to make the display of this assignment smoother, I had to reduce the amount of data and also remove the effect of clicking on an individual legend to hide the corresponding data.</p>
</div>
