---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
---
  <div style="position: relative;">
  <img src="assets/img/DTU_Logo_Corporate_Red_RGB.png" alt="Site logo" width="100" height="146" style="position: absolute; top:-230px;" class="sitelogo" />
  </div>

<head>
<link rel="icon" href="assets/img/DTU_Logo_Corporate_Red_RGB.png" sizes="32x32">
<link rel="icon" href="assets/img/DTU_Logo_Corporate_Red_RGB.png" type="image/png" sizes="16x16">
<link rel="apple-touch-icon" href="assets/img/DTU_Logo_Corporate_Red_RGB.png">
<link rel="shortcut icon" href="assets/img/DTU_Logo_Corporate_Red_RGB.png" type="image/png">
</head>
  
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Profile Cards</title>
<style>
  .container {
    display: flex; /* 使用flex布局 */
    justify-content: space-around; /* 子元素平均分布在容器中 */
    align-items: left; /* 垂直居中对齐 */
    background-color: #f2f2f2;
    #border-radius: 10px;
    #padding: 10px;
    max-width: 600px;
    margin: auto;
  }
  .profile {
    display: flex; /* 使用flex布局 */
    align-items: center; /* 垂直居中对齐 */
  }
  .avatar {
    width: 106px;
    height: 106px;
    #border-radius: 50%; /* 圆形头像 */
    #margin-right: 10px;
        border: none;           /* 移除边框 */
      box-shadow: none;       /* 移除阴影 */
      -webkit-box-shadow: none;
      -moz-box-shadow: none;
      -o-box-shadow: none;
      -ms-box-shadow: none;
  }
  .role,.name {
    margin: 0;
  }
    .role {
    font-size: 14px;
      font-weight: 500;
     font-family: 'Lucida Grande', 'Calibri', Helvetica, Arial, sans-serif;
    color: #777;
  }
  .name {
    font-size: 14px;
    font-weight: 500;
    font-family: 'Lucida Grande', 'Calibri', Helvetica, Arial, sans-serif;
    color: #333;
  }
</style>
</head>
<body>

<div class="container">
  <div class="profile">
    <img class="avatar" src="assets/img/zdyr.png" alt="Contributor Avatar">
    <div>
      <div class="name">@Danyiran Zhang_S232260</div>
      <div class="role">CONTRIBUTOR</div>
    </div>
  </div>
  <div class="profile">
    <img class="avatar" src="assets/img/2.png" alt="Teacher Avatar">
    <div>
      <div class="name">@Sune Lehmann Jørgensen</div>
      <div class="role">TEACHER</div>
    </div>
  </div>
</div>

</body>
</html>

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
  <img src="assets/img/crimes_per_hour_of_the_week.png" alt="Number of Crimes per Hour of the Week by Category" class="img1"/>
  <p>Each crime type shows a pattern of crime distribution over the course of a week, and it can be seen that certain crimes have a distinct high incidence period at certain times.</p>
  <p>The spikes in some charts are higher than others, suggesting that some types of crime are more common than others. The number of burglaries, for example, is significantly higher than cases of drunkenness or drugs.</p>
  <p>Such information could be particularly useful for law enforcement agencies in crime prevention and resource allocation, as it could guide them to step up policing at specific times of the week.</p>
  <p>At the same time, it is also very good information for people living in the nearby communities, and they can make targeted measures based on this information to protect themselves and their families.</p>
  <h2>Ⅱ Visualizing geodata</h2>
  <embed
   type="text/html" 
   src="/assets/map.html" 
   width="800" 
   height="600"
   class="map1">
  <p>The colors for many areas can be very similar, making the visual differences less apparent." I try to use a logarithmic scale for color mapping, which would reduce the visual gap between high and low values, making the differences in mid-range values more pronounced. </p>
  <p>As a result, we can clearly see from the graph that parking in the Richmond area on Sundays is the safest, while the Southern area is the least safe for parking.</p>
  <h2>Ⅲ Interactive visualizations</h2>
  <embed
   type="text/html" 
   src="/assets/Interactive_visualization_small.html" 
   width="800" 
   height="600"
   class="map2">
  <p>Unfortunately, if we want to fully replicate the effect of clicking on the legend to hide data on this scatter plot, the overall size of the webpage would become very large, and the browsing speed would be very slow—even with a limited amount of data. Therefore, in order to make the display of this assignment smoother, I had to reduce the amount of data and also remove the effect of clicking on an individual legend to hide the corresponding data.</p>
  <p>This image is an interactive crime map that shows the geographic distribution of different crime types in San Francisco. Each color represents a type of crime, and each dot in the image represents a crime incident. We can observe the pattern of crime occurrence, the high incidence areas and the distribution of crime types. The legend lists various types of crimes and marks them with different colors, such as vehicle theft, assault, and robbery.
This graph also shows that the data density is high, with events occurring at almost every location.</p>
</div>

<div class="Realsituation-section">
<h1>Real situation</h1>
<p>In this website (https://abc7news.com/feature/san-francisco-bay-area-safety-tracker-crime-stats-how-safe-is-my-neighborhood-zip-code-statistics/12442207/) I found some relevant information (homicide rate), which is from 2020 through March 31, 2024, and the trend of the data on the graph is basically consistent with our second part: Richmond, PARK, TARAVAL, and INGLESIDE have not only a low crime rate, but also a low homicide rate.</p>
<img src="assets/img/A closer look at San Francisco homicides by neighborhood.png" alt="A closer look at San Francisco homicides by neighborhood" class="img2"/>
<p>The map color codes each neighborhood by the homicide rate over the last 12 months. The three darker blues highlight neighborhoods where the murder rate is higher than the citywide rate.</p>
<img src="assets/img/abc_news_2021.png" alt="2021 homicide rate comparison in select major cities" class="img3"/>
<p> Meanwhile, I can see in the last picture of this website that compared with other cities in the United States, San Francisco's homicide rate in 2021 is not very high, ranking among the lowest, indicating that San Francisco's security situation is relatively good in the United States.</p>
</div>

<div class="conclution-section">
<h1>Conclution</h1>
<p>Each crime type shows a pattern of crime distribution over the course of a week, and it can be seen that certain crimes have a distinct high incidence period at certain times.</p>
</div>

<div class="contribution-section">
<h1>Contribution</h1>
<p>Danyiran Zhang-S232260 is a LONE WOLF, so his contribution is 100%.</p>
</div>
