---
permalink: /
layout: archive
title: "Welcome!"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---



I am a Ph.D. candidate in [Sociology](https://soc.ucla.edu/) and an M.S. student in [Statistics and Data Science](https://statistics.ucla.edu/) at the University of California, Los Angeles (UCLA). I am affiliated with the [Inequality Data Science Lab (IDS-Lab)](https://www.inequalitydatasciencelab.org/) and the [California Center for Population Research (CCPR)](https://ccpr.ucla.edu/). Prior to UCLA, I worked in public policy think tanks, including the [Asian Development Bank Institute](https://www.adb.org/adbi/main) in Tokyo, Japan. I hold an M.P.P. from the University of Tokyo in Japan and a B.A. in Sociology from Ewha Womans University in South Korea, where I completed the [Scranton Honors Program](https://myr.ewha.ac.kr/escranton/shp/about-shp.do) with a focus in Society and Justice, an interdisciplinary academic track. 

## Research Interests 
------
My research focuses on the following interconnected areas: (1) the intersection of **social stratification** and **life course** studies, using **life disruptions** as critical lenses to examine inequality; (2) **intra-group inequality**, analyzing how intersecting socioeconomic resources create divergent outcomes within seemingly homogeneous groups; and (3) the advancement of **statistical and machine learning methods** for sociological research and causal inference.

My work has been published in several journals, including the _Journal for the Scientific Study of Religion_, _Journal of Marriage and Family_, and _Social Science Research_. My research has been recognized with funding and awards, including the [Donald J. Treiman Research Fellowship](https://ccpr.ucla.edu/funding/treiman-research-fellowship/) from the UCLA CCPR, the [Kawahara Fellowship](https://www.international.ucla.edu/japan/internal/4680), from the UCLA Terasaki Center for Japan Studies and a UCLA Dissertation Award. I have also received a nationally competitive scholarship from the [Kwanjeong Education Foundation](https://www.ikef.or.kr/) in Korea.

**I will be on the academic job market for the 2025–2026 academic year**, seeking tenure-track faculty positions in sociology or related fields, as well as postdoctoral opportunities. For further details about my research and teaching, please visit my [research](/research) and [teaching](/teaching) pages, or view my [CV](/files/CV_NJ.pdf).


## Recent News
------
<style>
  ul.news-list {
    list-style-type: none; /* Removes default bullet points */
    padding-left: 0; /* Removes default padding */
    margin-top: 30px; /* Adds top margin */
  }

  ul.news-list li {
    margin-bottom: 20px; /* Adds space between news blocks */
  }

  .news-content {
    display: block; /* Default visibility for 2024 news */
    padding-top: 0px; /* Adds spacing above content */
  }

  .news-content.hidden {
    display: none; /* Hidden by default for previous years */
  }

  .year-title {
    font-weight: bold; /* Makes the year title bold */
    font-size: inherit; /* Inherit from the parent container */
    margin-bottom: 5px; /* Adds spacing below the year title */
    cursor: pointer; /* Indicates that the title is clickable */
  }

  .news-content ul {
    list-style-type: none; /* Removes bullet points for inner lists */
    padding-left: 0; /* Removes padding for inner lists */
    margin: 0; /* Removes margin for inner lists */
  }

  .news-content ul li {
    margin-bottom: 5px; /* Adds spacing between items in the same block */
  }

  @media (max-width: 768px) { /* Adjusts for devices with width up to 768px */
    ul.news-list {
      margin-top: 20px; /* Reduces top margin on smaller screens */
    }
  }
</style>

<script>
  function toggle_visibility(event, id) {
    event.preventDefault();
    var element = document.getElementById(id);
    if (element.classList.contains('hidden')) {
      element.classList.remove('hidden');
    } else {
      element.classList.add('hidden');
    }
  }
</script>

<ul class="news-list">
  <!-- 2025 News - Visible by Default -->
  <li>
    <div class="news-content">
      <ul> 
        <li><b>Feb 2025:</b> I’m happy to share that I will be participating in the Max Planck Institute for Demographic Research's summer visit program in Rostock, Germany; my research will focus on machine learning for life course trajectory. </li>
        <li><b>Jan 2025:</b> I’m happy to share that I will be participating in a contributors’ workshop to present our review paper on causal machine learning for sociology for the 2026 special issue of Kölner Zeitschrift für Soziologie und Sozialpsychologie on 'Explanation and Causality in the Social Sciences' at Johannes Gutenberg University in April 2025. I am excited to gain new perspectives on causal inference and sociology and to connect with other scholars!</li>
      </ul>
    </div>
  </li>

  <!-- Old News - Hidden by Default -->
  <li>
    <div class="year-title" onclick="toggle_visibility(event, 'news-2024');">2024</div>
    <div id="news-2024" class="news-content hidden">
      <ul>
        <li><b>Dec 2024:</b> I’m excited to serve on the organizing team for next summer’s RC28 Meeting at UCLA. We’re looking forward to welcoming submissions and fostering meaningful discussions on social mobility and inequality among stratification researchers from around the world.</li>
        <li><b>Oct 2024:</b> I’m pleased to share that I’ll be organizing a regular session on Work and Family for ASA 2025. If you’re conducting research in this area, I’d be glad to see your work—please consider submitting.</li>
        <li><b>Feb 2024:</b> I’m grateful to have received UCLA’s dissertation award, which is supporting my research on life course inequalities.</li> 
      </ul>
    </div>
  </li>

  <li>
    <div class="year-title" onclick="toggle_visibility(event, 'news-2023');">2023</div>
    <div id="news-2023" class="news-content hidden">
      <ul>
        <li><b>June 2023:</b> I had the privilege of organizing SICSS-UCLA (Summer Institute in Computational Social Science) with a focus on causal inference. It was an inspiring experience to connect with scholars passionate about leveraging computational methods for social science research. Learn more about SICSS here: <a href="https://sicss.io">https://sicss.io</a>.</li>
      </ul>
    </div>
  </li>
</ul>





