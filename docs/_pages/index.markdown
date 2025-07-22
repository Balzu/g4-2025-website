---
layout: dark_layout
title: "Home"
show_sidetoc: true
header_type: hero
header_img: assets/images/cyber_attacks_world_hd.gif
header_title: "The Italian Job… of Cybercrime"
subtitle: "Data, Emotions, and Investments in the Cyber War"
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


<div>
  <vegachart
    schema-url="{{ "/assets/charts/map_the_attack/attori_europa_black.json" | relative_url }}"
    style="width: 100%; height: 100%" 
    tooltip="true" >
  </vegachart>
</div>


<div>
  <vegachart
    schema-url="{{ "/assets/charts/map_the_attack/average_trend_italy_europe_black.json" | relative_url }}"
    style="width: 100%; height: 100%" 
    tooltip="true" >
  </vegachart>
</div>


<div>
  <vegachart
    schema-url="{{ "/assets/charts/map_the_attack/cloropleth_blu_verde_black.json" | relative_url }}"
    style="width: 100%; height: 100%" 
    tooltip="true" >
  </vegachart>
</div>


<div>
  <vegachart
    schema-url="{{ "/assets/charts/map_the_attack/duration_gangs_italy_ok_prova1_black.json" | relative_url }}"
    style="width: 100%; height: 100%" 
    tooltip="true" >
  </vegachart>
</div>


<div>
  <vegachart
    schema-url="{{ "/assets/charts/map_the_attack/industry_size_italy_black.json" | relative_url }}"
    style="width: 100%; height: 100%" 
    tooltip="true" >
  </vegachart>
</div>


<div>
  <vegachart
    schema-url="{{ "/assets/charts/map_the_attack/rank_italy_attack_count_black.json" | relative_url }}"
    style="width: 100%; height: 100%" 
    tooltip="true" >
  </vegachart>
</div>


<div>
  <vegachart
    schema-url="{{ "/assets/charts/map_the_attack/settori_colpiti_italy_black.json" | relative_url }}"
    style="width: 100%; height: 100%" 
    tooltip="true" >
  </vegachart>
</div>


<div>
  <vegachart
    schema-url="{{ "/assets/charts/map_the_attack/trend_black.json" | relative_url }}"
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


1.media_coverage_cyberattacks.json
<div>
  <vegachart
    schema-url="{{ "/assets/charts/breaking_the_net/1_aziende/1.media_coverage_cyberattacks.json" | relative_url }}"
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

## Research vs. Reality: Italy’s Cybersecurity Investments Under the Microscope  

Over the last decade, Italy has steadily climbed the European cybersecurity ladder — at least on paper. According to data from Horizon 2020 and Horizon Europe, the country ranks third in terms of net cybersecurity funding received, behind only Spain and Germany. From 2015 onward, Italy’s involvement in EU-backed research projects has grown consistently, peaking in 2021 with **115 active initiatives.**  

This trajectory suggests a country that, even before the surge in cyberattacks, was aware of the need to strengthen its digital defenses — a sign of strategic foresight in the face of accelerating digitalization.  

But while the research ecosystem expanded, so did the threats. **In 2023, Italy recorded its highest-ever number of cyberattacks against companies,** continuing a trend that began around 2021 — the same period during which funding reached its peak.  

This overlap raises a critical and still unresolved question:  

### Are these investments paying off in the real world?  

At present, the answer is unclear. It’s possible the benefits of funding are simply delayed — that training, infrastructure, and innovation need time to convert into effective defense mechanisms. But another possibility looms: that **the translation of research into operational security is too slow, too fragmented, or even misaligned** with the actual needs of Italian businesses.  

This isn’t just a budgeting issue — it’s a structural one. The numbers tell one story, but they also invite a deeper investigation:  

### Does Italy’s cybersecurity model need a rethink? And if so, where should we start?  

To explore this further, we asked a **senior academic figure**  for their honest view on the situation. Here's what they shared:  

>As far as I know, the increase in projects hasn’t brought any significant or visible benefits. It mainly reflects better organizational capacity in the Italian ecosystem to apply for and manage funds. I haven’t seen more strategic selection of projects, nor clear impact in terms of cybersecurity outcomes or the emergence of new actors in the field.  
>For example, Spain has focused its funding on building infrastructure and labs. In contrast, in Italy, a large portion of funds has gone toward increasing precarious or part-time roles in public and private organizations. In the short term, this boosts fund usage rates, but in the long term, it brings little benefit — and even creates social costs, as we’re seeing in the academic sector.

His words offer an honest reflection — and leave us with a crucial, open-ended question:  

Will these investments eventually strengthen Italy’s cybersecurity landscape, or do we need to rethink how research is connected to real-world needs and resilience?” 

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