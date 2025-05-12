---
layout: page
title: "Once Upon a Time in Hollywood: Movie Genres Through Time"
subtitle: "A final project for 02806 Social Data Analysis and Visualization"
---

---

<div style="display: flex; align-items: center; gap: 2rem; margin-top: 2rem;">

  <!-- Text block -->
  <div style="flex: 1;">
    <h2>Introduction</h2>
    <p>
      Film has existed as a medium for well over a century. From black-and-white silent films to today’s global blockbusters, one thing remains: we keep watching. 

      We all have our favorites, but there might be hidden patterns we’re not aware of. Maybe you’re watching more action films than you think. Or perhaps there’s a genre that connects viewers across the world.
    </p>
  </div>

  <!-- Image block -->
  <div style="flex: 1; max-width: 300px;">
    <img src="{{ '/assets/img/imdb.png' | relative_url }}" alt="IMDb logo" style="width: 100%; border-radius: 8px;">
  </div>

</div>

This article explores how movie genres have evolved over the last hundred years. Are some genres timeless, or do they come and go with the decades? How do major world events affect movie preferences? And do certain regions favor specific types of films? 
By looking at these patterns, we will see how film not only entertains but also reflects the cultural shifts, societal values, and global events that shape our world.


<h3> The dataset </h3> 


The dataset used in this article is derived from the **Internet Movie Database (IMDb)**, a publicly available collection of metadata about movies (and other visual media). It includes structured information such as movie titles, release years, runtime, genre classifications, and user ratings. The data is updated daily by IMDb and provides a comprehensive foundation for analyzing trends and patterns in the global film industry.

## Focusing the Lens  (10 focus genres)

There are many sub-genres in the world of film. Over time, new combinations have emerged. Some could perhaps be considered a bit niche - like “scandi-noir-crime” or “bumbling-detective-mystery”  [2]. While these subgenres are certainly entertaining, they may mutter the objective. 

To keep things clear, we’ve narrowed our scope. We’re looking at the ten most popular main-genres in the dataset: Action, Adventure, Comedy, Crime,  Documentary, Drama, Horror, Mystery, Romance and Thriller. As these are genre tags, some movies will have more than one genre. In these situations, they will be included in both categories.

<h2> Film genre throughout time </h2> 

<figure style="text-align: left; margin: 2em 0;">
  <div style="width: 120%; max-width: 120%; overflow: hidden;">
    <div style="transform: scale(0.8); transform-origin: top left; width: 125%; height: 560px;">
      <iframe 
        src="{{ '/plots/interactive_movie_genre_distribution.html' | relative_url }}"
        style="width: 120%; height: 700px; border: none;"
        title="InteractiveDistribution"
      ></iframe>
    </div>
  </div>
  <figcaption style="font-size: 0.95rem; color: #777; margin-top: 0.5em;">
    Figure 1. The visualization above presents a dual view of the film industry’s evolution: the total number of movies produced each year (top, in grey bars), and the proportional distribution of ten major genres (bottom, as a stacked area chart)
  </figcaption>
</figure>

As the annual movie production reveals, there’s been a steady increase in movie production since the 2000s. Unsurprisingly, this trend experienced a slight drop around 2020 during COVID-19,  which made production companies put projects on hold [2].
The distribution of movie genres has changed over the last hundred years. In the 1920s, romance made up about 20% of all films. Today, it is around 6%. Genres like documentary, horror, and thriller were rare in the past. Now, they make up 7-15% of all movies.

The rise in documentaries since the 1990s can perhaps be linked to the availability of cheaper and smaller video cameras. Hand-held cameras and DSLRs may have lowered the barriers to making films: lower costs opening up the genre to non-professionals. In addition, documentaries offer the flexibility to cover a wide range of topics and personal experiences in many different settings [3][4]

The rise in genres like horror and thriller since the 1970s may be linked to broader historical and psychological factors. Some researchers propose that these genres become more popular during uncertain times, such as wars, political instability, or global crises like climate change. Stressful events might affect how people think and feel, leading audiences to seek out stories that deal with fear, tension, and the unknown. This idea may help explain the increase in horror and thriller films during the Cold War and again today, in response to the pandemic and climate concerns [5].

While we've seen how different genres have evolved over time and across regions, another key question arises: how do these genres differ in terms of viewer reception and production style? To explore this, we examine the average IMDb rating across genres (Figure 2).

<figure style="text-align: left; margin: 2em 0;">
  <div style="width: 120%; max-width: 120%; overflow: hidden;">
    <div style="transform: scale(0.8); transform-origin: top left; width: 125%; height: 560px;">
      <iframe 
        src="{{ '/plots/average_imdb_rating_by_genre.html' | relative_url }}"
        style="width: 120%; height: 700px; border: none;"
        title="InteractiveDistribution"
      ></iframe>
    </div>
  </div>
  <figcaption style="font-size: 0.95rem; color: #777; margin-top: 0.5em;">
    Figure 2. Average IMDb rating and runtime for the different genres. 
  </figcaption>
</figure>

From this plot, we see that Documentaries stand out with the highest average rating (7.2), followed by Drama (6.3) and Romance (6.1). On the other end of the spectrum, Horror has the lowest average rating at 4.8, perhaps due to its divisive nature or the prevalence of low-budget productions within the genre. These results suggest a divide between genres associated with emotional depth or factual storytelling (like Drama and Documentary) and genres often centered around thrills or spectacle (like Action and Horror). 

The plot also shows the average runtime for each genre. Interestingly, documentaries — while rated the highest — are the shortest on average, typically under 80 minutes. Romance films, which also perform well in terms of ratings, have the longest runtimes, tied with action movies at 101 minutes. This contrast highlights how different genres balance depth and duration, suggesting that runtime alone isn’t a clear indicator of audience appreciation.

<h2> An overview of film production around the world </h2> 

<figure style="text-align: left; margin: 2em 0;">
  <div style="width: 120%; max-width: 120%; overflow: hidden;">
    <div style="transform: scale(0.78); transform-origin: top left; width: 125%; height: 585px;">
      <iframe 
        src="{{ '/plots/interactive_genre_map.html' | relative_url }}"
        style="width: 120%; height: 750px; border: none;"
        title="InteractiveDistribution"
      ></iframe>
    </div>
  </div>
  <figcaption style="font-size: 0.95rem; color: #777; margin-top: 0.5em;">
    Figure 3. Interactive map of genres throughout the world. Interact by choosing a genre in the top bar and seeing it's strength in each country. 
  </figcaption>
</figure>

<h2> Weekly movie releases </h2> 

<figure style="text-align: left; margin: 2em 0;">
  <div style="width: 120%; max-width: 120%; overflow: hidden;">
    <div style="transform: scale(0.78); transform-origin: top left; width: 120%; height: 820px;">
      <iframe 
        src="{{ '/plots/interactive_movie_releases_polar.html' | relative_url }}"
        style="width: 120%; height: 1280px; border: none;"
        title="InteractiveDistribution"
      ></iframe>
    </div>
  </div>
  <figcaption style="font-size: 0.95rem; color: #777; margin-top: 0.5em;">
    Figure 4. Stacked genre plot throughout the year. Choose a genre in the drop down list in the top left, and viewing its release distribution through an average year.
  </figcaption>
</figure>

