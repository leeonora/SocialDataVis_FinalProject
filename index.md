---
layout: page
title: "Once Upon a Time in Hollywood"
subtitle: "A final project for 02806 Social Data Analysis and Visualization"
---
<p class="subtitle">How Movie Genres Reflect the World</p>

<div style="background-color: #fff3cd; border-left: 6px solid #ffeeba; padding: 1rem; margin-bottom: 1.5rem;">
  <strong>Note:</strong> The plots on this website may take up to two minutes to load due to their size and complexity. Thank you for your patience!
</div>

---
<div style="display: flex; align-items: center; gap: 1rem; margin-top: 0.1rem;">
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

This article explores how movie genres have evolved over the last hundred years. Are some genres timeless, or do they come and go with the decades or seasons? How do major world events affect movie preferences? And do certain regions favor specific types of films? 
By looking at these patterns, we will see how film not only entertains but also reflects the cultural shifts, societal values, and global events that shape our world.


<h3> The dataset </h3> 

The dataset used in this article is derived from the [Internet Movie Database (IMDb)](https://developer.imdb.com/non-commercial-datasets/?fbclid=IwY2xjawKQBbpleHRuA2FlbQIxMABicmlkETFtOXhTbmdaeGdPUWdtU2hDAR7XfZjy0YefLSthSVuhQBabTk_ywX-fIyK--ADp3tpJqZNh5D1MQfTw5OvYhA_aem_s8D-J0jPxTIMlezCH6FTPg), a publicly available collection of metadata about movies (and other visual media). It includes structured information such as movie titles, release years, runtime, genre, location and user ratings.

For more information, visit the explainer notebook at the bottom of this page. 

## Focusing the Lens

There are many sub-genres in the world of film. Over time, new combinations have emerged. Some could perhaps be considered a bit niche, like “scandi-noir-crime” or “bumbling-detective-mystery”  [1]. While these subgenres are certainly entertaining, they may mutter the objective. 

To keep things clear, we’ve narrowed our scope. We’re looking at the ten most popular main genres in the dataset: Action, Adventure, Comedy, Crime,  Documentary, Drama, Horror, Mystery, Romance and Thriller. As these are genre tags, some movies will have more than one genre. In these situations, they will be included in both categories.

<div style="background-color: #fff3cd; border-left: 6px solid #ffeeba; padding: 1rem; margin-bottom: 1.5rem;">
  <strong>Note:</strong> All figures in this article are interactive plots created using Plotly. We encourage you to explore the data by zooming, hovering and selecting genres from the legends. 
</div>

<h2> About Time: Film Genre Throughout the Years </h2> 

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
    Figure 1. The visualization above presents a dual view of the film industry’s evolution: the total number of movies produced each year (top, in grey bars), and the proportional distribution of ten focus genres (bottom, as a stacked area chart).
  </figcaption>
</figure>

As the annual movie production reveals, there’s been a steady increase in movie production since the 2000s. Unsurprisingly, this trend experienced a slight drop around 2020 during COVID-19,  which made production companies put projects on hold [2].
The distribution of movie genres has changed over the last hundred years. In the 1930s, romance made up about 14% of all films. Today, it is around 5%. Genres like documentary, horror, and thriller were rare in the past. Now, they make up 7-15% of all movies.

The rise in documentaries since the 1990s can perhaps be linked to the availability of cheaper and smaller video cameras. Hand-held cameras and DSLRs may have lowered the barriers of film-making: lower costs opening up the genre to non-professionals. In addition, documentaries offer the flexibility to cover a wide range of topics and personal experiences in many different settings [4][5].

The rise in genres like horror and thriller since the 1970s may be linked to broader historical and psychological factors. Some researchers propose that these genres become more popular during uncertain times, such as wars, political instability, or global crises like climate change. Stressful events might affect how people think, leading audiences to seek out stories that deal with fear, tension, and the unknown. This idea may help explain the increase in horror and thriller films during the Cold War and again today, in response to the pandemic and climate concerns [6].

While we've seen how different genres have evolved over time, another key question arises: how do these genres differ in terms of viewer reception and production style? To explore this, we examine the average IMDb rating and runtime across genres (Figure 2).

<figure style="text-align: left; margin: 2em 0;">
  <div style="width: 120%; max-width: 120%; overflow: hidden;">
    <div style="transform: scale(0.8); transform-origin: top left; width: 125%; height: 500px;">
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

The plot also shows the average runtime for each genre. Interestingly, documentaries, while rated the highest, are the shortest on average. Romance films, which also perform well in terms of ratings, have the longest runtimes. This suggests that runtime alone isn’t a clear indicator of audience appreciation.


> **To see the specific top 10 movies for each genre...**  
> Check out our [supporting page](https://fvhreimert.github.io/top_10_movies_soc_data/?fbclid=IwZXh0bgNhZW0CMTAAYnJpZBExbTl4U25nWnhnT1FnbVNoQwEe7-jfbjJA0nXy9oF2XVK2_BkS0sMcVW0iTrF3eqRkWkfty_MwRUGmwjO9Pog_aem_K70c36IL4lC7bxMHN2HcDA) (filtered to movies with 30,000+ votes).


<h2> Lost In Translation: An Overview of Film Production Around the World </h2> 

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
    Figure 3. Interactive map of genre specialization throughout the world. Interact by choosing a genre in the top bar and viewing it's strength in each country. 
  </figcaption>
</figure>

We’ve seen how genres change over time. But perhaps the genre popularity within a country can reflect its culture and audience. The map in Figure 3 shows how genre preferences vary across the world.

From this figure it becomes evident that there is largely a similar share of film genres between countries. However, some countries show a strong tendency towards a specific genre.

For instance, the map reveals that 25% of all movies produced in Cambodia are of the Horror genre. This ranks Cambodia as the country with the biggest share of horror films world-wide. A quick Google search confirms that horror is especially popular among Cambodian youth, often influenced by their own myths and folklore [9].

Another notable mention is Iceland, where more than half of film production is documentaries. This trend might be due to several factors. Iceland has a small population, and is known for its unique landscape, commercially referred to as “the land of fire and ice” [11]. To attract filmmakers, the Icelandic government offers up to 35% in tax refunds on film production. Furthermore, institutions such as the Icelandic Film Centre hosts film festivals and supports Icelandic filmmakers with funding and grants [7][8]. Thus, a small population, tax refunds and accessible funding might explain why this country is ideal for documentaries. 

The overview also helps to debunk some common assumptions. For instance, you might think Hollywood equals blockbuster action films. But in reality, they only cover around 8% of the US market.

<h2> The Four Seasons: Release Trends During A Year</h2> 

Figure 4 shows how film releases from 1980 to the present day are distributed throughout the calendar year. The plot is interactive, and can be filtered by genre. It is also possible to aggregate by weekly, monthly or daily release patterns, using the buttons at the bottom center. Beware that when aggregating by day, an abundance of movie release dates default to the first of the month due to the nature of the dataset (this does not necessarily reflect true release dates). 

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
    Figure 4. Stacked polar bar chart. Choose one or more genres by clicking on them in the legend, and viewing their release distribution throughout the year since 1980. Select monthly, weekly or daily data in the bottom center. 
  </figcaption>
</figure>

The yearly release pattern reveals a pronounced peak in film releases during the fall months. As summer fades, audiences are more likely to return to the cinemas, no longer distracted by outdoor activities. October stands out as a particularly busy month for horror, crime and thiller releases, while romance films hit their peak in September. Surprisingly not around Valentine's Day, but rather at the start of "cuffing season", during which the general population tends to look for a partner to spend the colder months watching movies with [12].

In contrast, the winter months January and February see the lowest release numbers, reinforcing their reputation as "Dump Months", a term referring to a time when studios traditionally avoid releasing their major blockbusters. Several factors contribute to this pattern, including competition from other forms of entertainment (e.g., the Super Bowl), eligibility rules for the Academy Awards, and the economic strain on households after the holiday spending spree [10].

While August and September are also commonly considered "Dump Months," this is not fully reflected in the data. In fact, the plot suggests that July may be more accurately categorized as such, likely due to the absence of many families on vacation.

On a weekly basis, weeks 36 and 40 show the highest average number of releases. This could be due to the lead-up to the fall holidays, such as Thanksgiving and other significant breaks, like Columbus Day, during which studios capitalize on increased leisure time.

<h2> Final Destination: Conclusion </h2>

Looking at the data, a few things stand out. Movie genres shift over time (some rise, some fade) and some of these changes line up with what’s happening in the world. Horror and thriller get more popular during tense periods, while documentaries seem to benefit from better tech and wider access.

Genre preferences across countries are surprisingly consistent, with notable outliers like Cambodia’s love for horror or Iceland’s focus on documentaries.

Finally, release timing clearly isn’t random. Fall is the busiest season, while winter (especially January and February) tends to be the quietest.

In short: movie genres reflect more than just what people like to watch. They reflect when, where, and why we watch them, too.

---
<h2> The (Explainer) Notebook </h2>

[Click to view the explainer notebook](https://nbviewer.org/github/leeonora/SocialDataVis_FinalProject/blob/main/explainer_notebook.ipynb)

[or find it in our repository](https://github.com/leeonora/SocialDataVis_FinalProject/blob/main/explainer_notebook.ipynb)


---

<h3> References </h3>

[1] https://help.imdb.com/article/contribution/titles/keywords/GXQ22G5Y72TH8MJ5?ref_=helpart_nav_30#subgenres

[2] https://www.theguardian.com/film/2020/dec/21/how-covid-19-upturned-film-in-2020

[4] https://www.theguardian.com/film/2011/jun/06/new-technology-documentary-making

[5]
https://www.researchgate.net/publication/331320440_The_DSLR_Revolution_and_its_Impact_on_Documentary_and_Ethnographic_Filmmaking

[6] https://www.psychologytoday.com/us/blog/the-asylum/202308/war-and-the-horror-genre

[7]https://filminiceland.com/incentives-to-film-in-iceland/

[8]https://www.icelandicfilmcentre.is/about/icelandic-film-industry-at-a-glance

[9]https://www.kongchak.com/from-angkor-wat-to-aps-haunts-a-khmer-horror-film-odyssey/

[10] https://tvtropes.org/pmwiki/pmwiki.php/Main/DumpMonths 

[11] https://www.icelandair.com/

[12] https://www.merriam-webster.com/wordplay/cuffing-season-meaning-origin