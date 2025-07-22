---
layout: dark_layout
title: "Home"
show_sidetoc: true
header_type: hero
header_img: assets/images/cyber_attacks_world_hd.gif
header_title: "The Italian Job… of Cybercrime"
subtitle: "Italy Under Attack: Data, Emotions, and Investments in the Cyber War"
vega: true  
---

<style>
  /* Full‑page hero background */
  .site-hero {
    height: 100vh;
    background-image: url('{{ page.header_img | absolute_url }}');
    background-size: cover;
    background-position: center center;
    background-repeat: no-repeat;
  }
  .site-hero .hero-content {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    color: #fff;
    text-shadow: 0 0 10px rgba(0,0,0,0.7);
  }

  .vg-tooltip,
  .vg-tooltip .value,
  .vg-tooltip .key {
    color: #000 !important;
  }

.hm-buttons {
  display:flex;
  gap:.5rem;
  margin-bottom:1rem;
  flex-wrap:wrap;
}
.hm-btn {
  cursor:pointer;
  padding:.5rem .9rem;
  border:1px solid #ccc;
  background:#f5f5f5;
  border-radius:4px;
  font-size:.9rem;
}
.hm-btn.active {
  background:#d33;
  color:#fff;
  border-color:#d33;
}
.heatmap { display:none; }
.heatmap.visible { display:block; }

div aside {
    background-color: #000000;
}

.container-lg {
    background-color: #000000 !important;
}

canvas {
    max-width: 100% !important;
}

</style>


# Introduction {#introduction}

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incidunt ut labore et dolore magna aliqua.


<div>
  <vegachart
    schema-url="{{ "/assets/charts/intro/1.bottone_reddit_sentiment_trend.json" | relative_url }}"
    style="width: 100%; height: 100%"
    tooltip="true" >
  </vegachart>
</div>



<div>
  <vegachart
    schema-url="{{ "/assets/charts/intro/2.bottone_reddit_normalized_comments.json" | relative_url }}"
    style="width: 100%; height: 100%"
    tooltip="true" >
  </vegachart>
</div>



<div>
  <vegachart
    schema-url="{{ "/assets/charts/intro/3.emotion_distribution_reddit_dropdown.json" | relative_url }}"
    style="width: 100%; height: 100%"
    tooltip="true" >
  </vegachart>
</div>




# Map the Attack {#map-the-attack}

![Infografica]({{ "/assets/images/infografica.png" | relative_url }})

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incidunt ut labore et dolore magna aliqua.


<div class="hm-buttons">
  <button type="button" class="hm-btn active" data-target="heatmap1">Attacks per Region</button>
  <button type="button" class="hm-btn" data-target="heatmap2">Attacks / Revenue</button>
  <button type="button" class="hm-btn" data-target="heatmap3">Attacks / Companies</button>
</div>

<div id="heatmap1" class="heatmap visible">
  <vegachart
    schema-url="{{ "/assets/charts/heatmap1.json" | relative_url }}"
    style="width: 100%; height: 100%" 
    tooltip="true" >
  </vegachart>
</div>

<div id="heatmap2" class="heatmap">
  <vegachart
    schema-url="{{ "/assets/charts/heatmap2.json" | relative_url }}"
    style="width: 100%; height: 100%" 
    tooltip="true" >
  </vegachart>
</div>

<div id="heatmap3" class="heatmap">
  <vegachart
    schema-url="{{ "/assets/charts/heatmap3.json" | relative_url }}"
    style="width: 100%; height: 100%" 
    tooltip="true" >
  </vegachart>
</div>

duration_gangs_italy_OK_PROVA1_BLACK.json
<div>
  <vegachart
    schema-url="{{ "/assets/charts/map_the_attack/duration_gangs_italy_OK_PROVA1_BLACK.json" | relative_url }}"
    style="width: 100%; height: 100%" 
    tooltip="true" >
  </vegachart>
</div>


<div>
  <vegachart
    schema-url="{{ "/assets/charts/map_the_attack/financing/ita_eu_average_fino_23_arancio.json" | relative_url }}"
    style="width: 100%; height: 100%" 
    tooltip="true" >
  </vegachart>
</div>


<div>
  <vegachart
    schema-url="{{ "/assets/charts/map_the_attack/financing/italy_active_projects_per_year.json" | relative_url }}"
    style="width: 100%; height: 100%" 
    tooltip="true" >
  </vegachart>
</div>


<div>
  <vegachart
    schema-url="{{ "/assets/charts/map_the_attack/2025_cloroplet_blues.json" | relative_url }}"
    style="width: 100%; height: 100%" 
    tooltip="true" >
  </vegachart>
</div>


<div>
  <vegachart
    schema-url="{{ "/assets/charts/map_the_attack/actor_industry_finale.json" | relative_url }}"
    style="width: 100%; height: 100%" 
    tooltip="true" >
  </vegachart>
</div>

actor_presence_ita_eu_arancio.json:
<div>
  <vegachart
    schema-url="{{ "/assets/charts/map_the_attack/actor_presence_ita_eu_arancio.json" | relative_url }}"
    style="width: 100%; height: 100%" 
    tooltip="true" >
  </vegachart>
</div>


<div>
  <vegachart
    schema-url="{{ "/assets/charts/map_the_attack/duration_gangs_italy_ok_prova1.json" | relative_url }}"
    style="width: 100%; height: 100%" 
    tooltip="true" >
  </vegachart>
</div>


<div>
  <vegachart
    schema-url="{{ "/assets/charts/map_the_attack/ita_eu_average_fino_23_arancio.json" | relative_url }}"
    style="width: 100%; height: 100%" 
    tooltip="true" >
  </vegachart>
</div>


<div>
  <vegachart
    schema-url="{{ "/assets/charts/map_the_attack/ita_eu_world_fino_al_2025_arancio.json" | relative_url }}"
    style="width: 100%; height: 100%" 
    tooltip="true" >
  </vegachart>
</div>


<div>
  <vegachart
    schema-url="{{ "/assets/charts/map_the_attack/ita_eu_world_fino_al_2025_arancio.json" | relative_url }}"
    style="width: 100%; height: 100%" 
    tooltip="true" >
  </vegachart>
</div>


<div> 
  <iframe src="{{ site.baseurl }}/assets/charts/map_the_attack/mappa_italia_aziende_hq_description.html" width="100%" height="400px" frameborder="0"></iframe> 
</div>


<div>
  <vegachart
    schema-url="{{ "/assets/charts/map_the_attack/settori_aziende_colpite_italia1.json" | relative_url }}"
    style="width: 100%; height: 100%" 
    tooltip="true" >
  </vegachart>
</div>


<div>
  <vegachart
    schema-url="{{ "/assets/charts/map_the_attack/trend_2023_no_undetermined.json" | relative_url }}"
    style="width: 100%; height: 100%" 
    tooltip="true" >
  </vegachart>
</div>


# Breaking the Net {#breaking-the-net}

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incidunt ut labore et dolore magna aliqua.

<div>
  <vegachart
    schema-url="{{ "/assets/charts/breaking_the_net/1_aziende/articles_by_source_type.json" | relative_url }}"
    style="width: 100%; height: 100%"
    tooltip="true" >
  </vegachart>
</div>

<div>
  <vegachart
    schema-url="{{ "/assets/charts/breaking_the_net/1_aziende/normalized_coverage_per_attack.json" | relative_url }}"
    style="width: 100%; height: 100%"
    tooltip="true" >
  </vegachart>
</div>

<div>
  <vegachart
    schema-url="{{ "/assets/charts/breaking_the_net/1_aziende/sentiment_by_industry.json" | relative_url }}"
    style="width: 100%; height: 100%"
    tooltip="true" >
  </vegachart>
</div>

1.average_sentiment_giornali_settore.json:
<div>
  <vegachart
    schema-url="{{ "/assets/charts/breaking_the_net/2_comparative/1.average_sentiment_giornali_settore.json" | relative_url }}"
    style="width: 100%; height: 100%"
    tooltip="true" >
  </vegachart>
</div>

<div>
  <vegachart
    schema-url="{{ "/assets/charts/breaking_the_net/2_comparative/2.sentiment_giornali_settore_2017_2024.json" | relative_url }}"
    style="width: 100%; height: 100%"
    tooltip="true" >
  </vegachart>
</div>

<div>
  <vegachart
    schema-url="{{ "/assets/charts/breaking_the_net/2_comparative/3.top_entities_sentiment_by_source.json" | relative_url }}"
    style="width: 100%; height: 100%"
    tooltip="true" >
  </vegachart>
</div>

<div>
  <vegachart
    schema-url="{{ "/assets/charts/breaking_the_net/2_comparative/4.most_frequent_tokens_by_source.json" | relative_url }}"
    style="width: 100%; height: 100%"
    tooltip="true" >
  </vegachart>
</div>

<div>
  <vegachart
    schema-url="{{ "/assets/charts/breaking_the_net/2_comparative/5.dominant_topic_sentiment_giornali_settore.json" | relative_url }}"
    style="width: 100%; height: 100%"
    tooltip="true" >
  </vegachart>
</div>


# Cyber Q&A {#cyber-q-and-a}


<iframe width="100%" height="400" src="https://www.youtube.com/embed/RI0W7NRl4SU?si=exRRIXoy2hr_qgFb&vq=hd1080" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>


<div> 
  <iframe src="{{ site.baseurl }}/assets/graph/top50_articles_mitre_graph.html" width="100%" height="400px" frameborder="0"></iframe> 
</div>




# Conclusions {#conclusions}

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incidunt ut labore et dolore magna aliqua.

<div>
  <vegachart
    schema-url="{{ "/assets/charts/conclusions/ita_eu_average_fino_23_arancio.json" | relative_url }}"
    style="width: 100%; height: 100%"
    tooltip="true" >
  </vegachart>
</div>


# About Us  {#about-us}

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incidunt ut labore et dolore magna aliqua.


<script>
document.querySelectorAll('.hm-btn').forEach(btn=>{
  btn.addEventListener('click', ()=>{
    const target = btn.dataset.target;

    document.querySelectorAll('.hm-btn').forEach(b=>b.classList.remove('active'));
    btn.classList.add('active');

    document.querySelectorAll('.heatmap').forEach(div=>div.classList.remove('visible'));
    document.getElementById(target).classList.add('visible');
  });
});
</script>