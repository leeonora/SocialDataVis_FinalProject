---
layout: page
Title: Back To The Future
---

<h1> Back To The Future: Movie Genres Through Time </h1> 

<h2> The dataset </h2> 

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

<h2> An overview of film genre throughout time </h2> 

<figure style="max-width: 100%; text-align: center; margin: 1em auto;">
  <iframe 
    src="/plots/interactive_movie_genre_distribution.html"
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
    src="/plots/interactive_genre_map.html"
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
    src="/plots/weekly_movie_releases_combined_stacked.html"
    style="width: 110%; height: 800px; border: none;"
    title="WeeklyCombined"
  ></iframe>
  <figcaption style="font-size: 0.95rem; color: #777; margin-top: 0.5em;">
    Figure 1. Plot
  </figcaption>
</figure>

