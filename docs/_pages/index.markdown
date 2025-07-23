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


<div>
  <vegachart
    schema-url="{{ "/assets/charts/map_the_attack/trend_black.json" | relative_url }}"
    style="width: 100%; height: 100%" 
    tooltip="true" >
  </vegachart>
</div>


Since 2020, the world has witnessed a sharp rise in cyber attacks, marking a **clear upward trend** that shows **no sign of slowing down**. This phenomenon spans across all continents, with **North America** experiencing the most pronounced growth—though it's worth noting that the dataset analyzed is U.S. based, which may partly explain the spike. **Europe follows** closely, highlighting the global scale of the threat and reinforcing the importance of a focused regional analysis. This escalation is closely linked to the **rapid digital transformation** triggered by the **COVID 19 pandemic**, which compelled organizations, institutions, and individuals to adopt digital technologies at an unprecedented pace—often without adequate cybersecurity safeguards—accelerating digital adoption by three to four years in many sectors ([eurofound.europa.eu](https://www.eurofound.europa.eu)). As we shift our focus to comparing trends within Europe, and specifically between Italy and the broader region, this context becomes especially relevant.


<div>
  <vegachart
    schema-url="{{ "/assets/charts/map_the_attack/rank_italy_attack_count_black.json" | relative_url }}"
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


Following this overview, a bar chart and a choropleth map of Europe offer a clearer picture of how cyber-attacks are ranked quantitatively by country and how they are geographically distributed across the region. **Italy** stands out as the second most targeted country in Europe, trailing only the United Kingdom—which recorded around 1,500 attacks compared to Italy’s approximately 900. The gap is significant, yet Italy clearly remains **a primary target**. Other major European powers like France, Germany, Spain, and Russia also rank among the top, though they fall behind Italy in total incidents. On a global scale, Italy still holds a prominent position, ranking **fourth** overall (after USA, UK and Canada). The United States dominates the landscape with a dramatically higher volume of attacks, underscoring both the scale of the threat and the importance of regional resilience.


<div>
  <vegachart
    schema-url="{{ "/assets/charts/map_the_attack/average_trend_italy_europe_black.json" | relative_url }}"
    style="width: 100%; height: 100%" 
    tooltip="true" >
  </vegachart>
</div>


When comparing Italy’s cyber-attack trend to the European average, a clear divergence emerges. In certain years—such as 2017—the numbers were nearly aligned, suggesting a comparable threat level. But shortly thereafter, Italy's curve began to rise steadily, with **sharp peaks** starting **around 2021**. This growth stands in stark contrast to the broader European trend, which remains more moderate—partly because many EU countries report very few incidents, in some cases fewer than 10, which pull the average down. This discrepancy underscores a pressing **need to focus attention on Italy**. While the continent as a whole faces growing cyber threats, Italy is experiencing a notably accelerated trajectory that demands specific, localized analysis and response. 
This brings us to the core of our investigation: **who is being targeted the most in Italy—and why?** To better understand this phenomenon, it's essential to first clarify the structure of the Italian corporate landscape. The characteristics of the national business ecosystem play a key role in shaping both the exposure and vulnerability of different actors. The overview below provides a snapshot of this landscape, setting the stage for a deeper analysis of attack patterns and motivations.


![Infografica]({{ "/assets/images/infografica.png" | relative_url }})

The infographic is based on data from **ISTAT (2022)** — not the most recent, but still a reliable reference for outlining the structure of Italian enterprises. According to this data, Italy hosts a large number of businesses, the vast majority of which are **micro** and **small enterprises**, making up **78.9%** and **18.5%** of the total, respectively. This overwhelmingly small-scale composition has important implications for cybersecurity readiness and resilience. In terms of geographic distribution, there is a clear regional divide: the **North of Italy dominates** in the number of companies with three or more employees. Specifically, the **North-West** accounts for **28.7%** of these businesses, while the **North-East** follows with **22.7%**. Unfortunately, up-to-date and detailed reports on the sectoral distribution of Italian companies are currently lacking, limiting a more granular analysis by industry. Nonetheless, this foundational overview helps contextualize **which types of organizations may be more exposed to cyber threats—and why.** 
Understanding this business structure is crucial, not only for assessing organizational readiness, but also for interpreting **how and where cyberattacks unfold across the country.** With this context in mind, we then turned our attention to the **geographic distribution of attacks** — evaluating not just their frequency, but how they correlate with the economic and structural makeup of each region.

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


When examining the distribution of attacks across Italian regions—both in terms of raw incident counts and data normalized by the number of companies and total regional revenue — **Lombardy** unsurprisingly emerges as the most targeted region during the timeframe considered in this study, followed by **Lazio**. Overall, cyberattacks appear to be more concentrated in **Northern Italy** — a trend that aligns with data from ISTAT, which shows that approximately **51%** of Italian companies are located in the northern regions. When examining the map normalized by the number of companies per region, the picture becomes even clearer: **Northern Italy appears more heavily targeted, likely because it simply hosts a larger volume of businesses, regardless of their size.**

However, Lazio still stands out. Even when adjusting for business density, it ranks as the most attacked region — suggesting that factors beyond company count are at play. One likely explanation is the high concentration of **public administration** entities headquartered in **Rome**, making Lazio a particularly attractive target for threat actors with political or ideological motives.

The picture shifts again when looking at attacks normalized by total regional revenue. In this case, Lazio continues to appear among the most affected, along with wealthy northern regions like Lombardy, Piedmont, and Emilia-Romagna. Interestingly, regions such as Umbria and some areas in Southern Italy — including Molise, Campania, and Basilicata — also emerge as disproportionately targeted. This suggests that, while these regions may host fewer companies, they might include large, high revenue enterprises that represent valuable targets for **financially motivated cybercriminals.** 

This foundational overview helps contextualize **which types of organizations may be more exposed to cyber threats — and why**. When analyzing our dataset of cyber-attacks in Italy, a clear pattern emerges: **the most targeted sector is Manufacturing, followed by Public Administration.**

This concentration of attacks on the manufacturing sector is likely tied to its **economic weight and increasing digitalization**, especially among **small and medium enterprises** that often lack mature cybersecurity protocols. According to the Cyber Index SME Report 2024 by Confindustria, Politecnico di Milano, and the Italian National Cybersecurity Agency, SMEs in Italy achieve a low average cyber-resilience score of just 52/100—highlighting widespread **gaps in risk awareness and security readiness.** At the European level, [ENISA](https://www.enisa.europa.eu/publications/enisa-report-cybersecurity-for-smes) has similarly noted that over 90% of SMEs adopted new digital tools during the pandemic without implementing additional cybersecurity measures. These vulnerabilities are further underscored by sector-specific analyses: in Italy, manufacturing alone accounted for over 13% of all cyberattacks in 2023—more than double its global share—making it a clear target for ransomware groups and threat actors focused on disrupting production or exfiltrating sensitive data (Muscope Manufacturing Cyber Risk Overview).


<div>
  <vegachart
    schema-url="{{ "/assets/charts/map_the_attack/settori_colpiti_italy_black.json" | relative_url }}"
    style="width: 100%; height: 100%" 
    tooltip="true" >
  </vegachart>
</div>


Together, these findings reflect a broader trend: cyber attackers tend to focus on sectors where **disruption can be maximized, and defenses are uneven** — highlighting systemic vulnerabilities that require urgent attention. This observation raises a critical question in the Italian context: **Are certain threat actors consistently targeting specific industries within the country — and if so, what drives these choices?** Identifying recurring patterns in attacker behavior can offer more than just a catalog of incidents. It can point to strategic intent—whether it's the exploitation of persistent vulnerabilities, economic sabotage, political motivations, or larger operations tied to ransomware or espionage campaigns. Understanding **who these actors are, how they operate, and which sectors they pursue most aggressively** is key to anticipating future risks. The following section delves into this aspect in greater detail, examining the activity of major threat actors in Italy and their preferred targets across different sectors. 



<div>
  <vegachart
    schema-url="{{ "/assets/charts/map_the_attack/actor_industry_finale.json" | relative_url }}"
    style="width: 100%; height: 100%" 
    tooltip="true" >
  </vegachart>
</div>

The plot highlights the intersection between **threat actors** and the **sectors** they most frequently target in Italy. From this analysis, several clear patterns emerge—both in terms of volume and strategic focus. **LockBit 3.0** stands out as the most prominent actor in terms of both volume and distribution of attacks, showing a clear preference for the manufacturing sector — which is, in fact, the most targeted sector in Italy. This correlation suggests a deliberate focus on **high-value industrial targets**, while notably, LockBit 3.0 appears to avoid the information sector almost entirely. A similar pattern is observed with its predecessor, **LockBit 2**, although this version shows a more even distribution across various sectors, with slightly higher activity in retail trade and lower interest in general services. In contrast, actors such as **Anonymous, Anonymous Italy, Noname057(16), LulzSecITA,** and **Killnet** seem to operate with a more **politically driven agenda**, primarily targeting public administration while largely ignoring the manufacturing sector. This behavior suggests an intention to **expose vulnerabilities** and **sensitive data** for demonstrative purposes, **rather than financial gain**, possibly exploiting known weaknesses or poorly secured access points within government institutions.



<div>
  <vegachart
    schema-url="{{ "/assets/charts/map_the_attack/duration_gangs_italy_ok_prova1_black.json" | relative_url }}"
    style="width: 100%; height: 100%" 
    tooltip="true" >
  </vegachart>
</div>


Looking at the timeline of activity for these threat actors in Italy further reinforces the patterns observed. As of 2025, only a few groups — **Akira, Cactus, 8Base, and Everest** — remain actively targeting Italian entities, suggesting a shift in the threat landscape or the **emergence** of new **ransomware-as-a-service** models. Notably, **Anonymous’** campaigns appear confined to a distinct period between 2015 and 2019, indicating that their influence in the Italian cyber threat environment has waned significantly over the past years. This temporal distribution also supports the hypothesis that LockBit 3.0 is a direct rebrand of the same group behind LockBit 2: LockBit 2’s activity visibly ends in June 2022, immediately followed by the first recorded attacks of LockBit 3.0 in July 2022. This seamless transition strongly implies operational continuity, not just in tactics but also in infrastructure and targeting logic — particularly the focused attention on the manufacturing sector discussed earlier.

As a final significant insight into the activity of these actors in Italy, an assessment was made to determine whether their operations are more **"generalist"** in nature — targeting multiple sectors across Europe — or if their focus is specifically on Italy. The analysis reveals that 14 out of the top 15 threat actors active in Italy also operate across the broader European landscape, suggesting a widespread, non-exclusive targeting strategy. The only exception is Sandworm, a notorious state-sponsored group linked to Unit 74455 of the Russian GRU. **Sandworm** has not been observed conducting operations in Italy, which aligns with its established profile: a highly sophisticated and destructive actor known for complex, coordinated cyberattacks, often aimed at critical infrastructure in **geopolitically strategic contexts**. Recognized by both MITRE ATT&CK and Western intelligence services as one of the most dangerous cyber threat actors globally, Sandworm’s absence from the Italian threat landscape may reflect its focus on targets deemed of higher strategic relevance to Russian state interests.


<div>
  <vegachart
    schema-url="{{ "/assets/charts/map_the_attack/attori_europa_black.json" | relative_url }}"
    style="width: 100%; height: 100%" 
    tooltip="true" >
  </vegachart>
</div>

This overview of sectoral and regional attack patterns underlines a clear reality: Italian businesses—particularly those in **manufacturing** and **public administration** — are at the epicenter of the national cyber threat landscape. Whether due to their economic weight, the sensitivity of the data they manage, or their uneven cybersecurity posture, these organizations present high-value opportunities for threat actors. At the same time, the geographic distribution of attacks closely mirrors the country's economic map, with Northern Italy—and to some extent, Lazio—bearing the brunt of cyber incidents.


These findings highlight a crucial point: **the cyber threat in Italy is not an abstract or distant phenomenon, but one that directly affects the core of its productive fabric**. And yet, **how visible is this risk to the broader public? To what extent has it penetrated mainstream discourse, and how is it being perceived by media and institutions?** The next section explores these questions, beginning with a look at how the presence of cyberattacks in Italy has evolved in public reporting over time.


**TODO**
<div>
  <vegachart
    schema-url="{{ "/assets/charts/map_the_attack/industry_size_italy_black.json" | relative_url }}"
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