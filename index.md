---
layout: page
Title: Back To The Future
---
<h1> Back To The Future: Movie Genres Through Time </h1> 
<h2> A final project for 02806 Social Data Analysis and Visualization </h2> 

<h2> Introduction </h2> 

Film has existed as a medium for well over a century. and throughout this time it has served as a reflection of society. From the golden age of Hollywood to the rise of elevated horror, movie genres and their popularity offer a window into which stories we have chosen to tell, and when. In this project, we explore the rise, change and popularities of film genres across the time and geography, as told by the comprehensive IMDb database. We hope to uncover interesting trends related to major world events (were apocalyptic sci-fi films more popular during the COVID-19 lockdown?) or changes in trends and preferences (were comedies more popular after the release of hit TV show Friends?), and thereby create a birds-eye view of how genres shift throughout the decades.  

<h3> The dataset </h3> 

The dataset used in this project is derived from IMDb Datasets, a publicly available collection of metadata about movies, TV shows, and other audiovisual content listed on the Internet Movie Database (IMDb). It includes structured information such as unique title identifiers, primary and original titles, release years, runtime, genre classifications, and user-generated ratings and votes. The data is updated daily by IMDb and provides a comprehensive foundation for analyzing trends and patterns in the global film and television industry.

<figure style="margin: 0;">
  <table style="margin: 0 auto; text-align: left; border-collapse: collapse;">
    <thead>
      <tr>
        <th>Column</th>
        <th>Description</th>
      </tr>
    </thead>
    <tbody>
      <tr><td>tconst</td><td>Unique identifier for the title (from IMDb)</td></tr>
      <tr><td>primaryTitle</td><td>The main title used for the movie/show</td></tr>
      <tr><td>originalTitle</td><td>The original title before translation/localization</td></tr>
      <tr><td>year</td><td>Year of release</td></tr>
      <tr><td>runtimeMinutes</td><td>Duration of the title in minutes</td></tr>
      <tr><td>genres</td><td>Genres assigned to the title (e.g., Comedy, Drama)</td></tr>
      <tr><td>rating</td><td>Average user rating</td></tr>
      <tr><td>votes</td><td>Total number of user votes</td></tr>
      <tr><td>country</td><td>Country of origin</td></tr>
    </tbody>
  </table>
  <figcaption style="text-align: left; font-size: 0.95rem; color: #777; margin-bottom: 0.5em;">
    Table 1. Column descriptions from the IMDb-based movie dataset.
  </figcaption>
</figure>

This project specifically focuses on exploring how film genres have evolved over time. Using a curated subset of the data, ten primary genres were selected for analysis: Drama, Comedy, Documentary, Romance, Action, Crime, Thriller, Horror, Adventure, and Mystery. Each genre is consistently represented by a distinct and relevant color throughout the visualizations to highlight changes in popularity, production frequency, and narrative focus across decades.

<h2> An overview of film genre throughout time </h2> 

<figure style="max-width: 100%; text-align: center; margin: 1em auto;">
  <iframe 
    src="{{ '/plots/interactive_movie_genre_distribution.html' | relative_url }}"
    style="width: 150%; height: 700px; border: none;"
    title="InteractiveDistribution"
  ></iframe>
  <figcaption style="font-size: 0.95rem; color: #777; margin-top: 0.5em;">
    Figure 1. Plot
  </figcaption>
</figure>

<h2> An overview of film genre throughout time </h2> 

<figure style="max-width: 100%; text-align: center; margin: 1em auto;">
  <iframe 
    src="{{ '/plots/interactive_genre_map.html' | relative_url }}"
    style="width: 160%; height: 800px; border: none;"
    title="InteractiveGenreMap"
  ></iframe>
  <figcaption style="font-size: 0.95rem; color: #777; margin-top: 0.5em;">
    Figure 1. Plot
  </figcaption>
</figure>

<h2> Weekly movie releases </h2> 

<figure style="max-width: 120%; text-align: center; margin: 1em auto;">
  <iframe 
    src="{{ '/plots/weekly_movie_releases_combined_stacked.html' | relative_url }}"
    style="width: 110%; height: 800px; border: none;"
    title="WeeklyCombined"
  ></iframe>
  <figcaption style="font-size: 0.95rem; color: #777; margin-top: 0.5em;">
    Figure 1. Plot
  </figcaption>
</figure>

