---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---
div class=<"magazine-style-intro">
  <h1>Welcome to Our Feature Article</h1>
  <p>This month's edition focuses on the vibrant intersections of technology and art, bringing you insights from industry leaders, innovative creators, and our expert team. Dive into our feature stories to explore the dynamic world of digital creation.</p>
</div>

<div class="content-section">
  <p>In San Francisco, a new research project is exploring the city's crime data to help the public understand the safety of their neighborhoods. The study's dataset is sourced from the official website of SF.gov at <a href="https://data.sfgov.org/">https://data.sfgov.org/</a>, a platform that centralizes data from multiple departments and public agencies with the goal of improving accessibility and efficiency of services while saving taxpayer dollars through the efforts of digital and data services teams.</p>
  <p>The dataset used in the study contains a wealth of column information, including case ID (PdId), Incident number (IncidntNum), incident code (Incident Code), Category, Descript, Day of the week, Date, Time, PdDistrict, Resolution, Address, coordinate X, coordinate Y, and location (location). With this data, researchers can conduct in-depth analyses to identify areas and time periods of high crime rates, as well as trends in specific crime types.</p>
  <p>Using data visualization tools such as Plotly, the researchers were able to map clearly which places are relatively safe and which are likely to require more public attention. This visual approach not only helps the public understand the security situation in the community, but also visually shows the areas where certain types of crime are most common, or when crime incidents are most common.</p>
  <p>In addition, most of the graphic design is designed to visually communicate information, such as by reading the bar chart, the public can quickly learn which types of crime incidents are the most frequent, and by visualizing the map, which areas are relatively safe or dangerous.</p>
  <p>It's worth noting that while the study covered data from 2003 to the end of 2017, the latest data is available from 2018 to the present on SF.gov. For readers interested in such studies, they can download the data directly to conduct their own analysis and research.</p>
  <p>Through the regional and temporal analysis of crime data, this project not only increases public awareness of community safety, but also provides a practical tool that enables people to make more informed decisions based on data, thereby improving their quality of life.</p>
</div>

<!-- Add this to your site's CSS file -->
<style>
.magazine-style-intro {
  max-width: 800px;
  margin: auto;
  padding: 20px;
  background-color: #f8f8f8;
  box-shadow: 0 4px 8px rgba(0,0,0,0.1);
  font-family: 'Georgia', serif;
}

.magazine-style-intro h1 {
  font-size: 2.5em;
  color: #333;
  margin-bottom: 0.5em;
}

.magazine-style-intro p {
  font-size: 1.2em;
  line-height: 1.6;
  color: #666;
}
</style>


<embed 
   type="text/html" 
   src="/assets/Interactive_visualization.html" 
   width="900" 
   height="600">
</embed>
