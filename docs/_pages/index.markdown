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


<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js" integrity="sha384-..." crossorigin="anonymous"></script>


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
.hm-btn1 {
  cursor:pointer;
  padding:.5rem .9rem;
  border:1px solid #ccc;
  background:#f5f5f5;
  border-radius:4px;
  font-size:.9rem;
}
.hm-btn1.active {
  background:#d33;
  color:#fff;
  border-color:#d33;
}
.hm-btn2 {
  cursor:pointer;
  padding:.5rem .9rem;
  border:1px solid #ccc;
  background:#f5f5f5;
  border-radius:4px;
  font-size:.9rem;
}
.hm-btn2.active {
  background:#d33;
  color:#fff;
  border-color:#d33;
}
.heatmap { display:none; }
.heatmap.visible { display:block; }

.barchart { display:none; }
.barchart.visible { display:block; }

div aside {
    background-color: #000000;
}

.container-lg {
    background-color: #000000 !important;
}

canvas {
    max-width: 100% !important;
}

strong {
    font-weight: 900 !important;
}

p a {
    color: #ca6701 !important;
}

.modal_link {
    color: #ca6701 !important;
}


.hm-btn1.active {
    background: #0a9396 !important;
    color: #fff;
    border-color: #0a9396 !important;
}
.hm-btn2.active {
    background: #0a9396 !important;
    color: #fff;
    border-color: #0a9396 !important;
}

a:hover {
  text-decoration: none !important; 
}

</style>


# Introduction {#introduction}

### Why Cybersecurity Matters — And Not Just for the Tech Industry 
_A breach might start with a keystroke — but its echo depends on who’s listening._ 

In today’s digital society, cybersecurity can no longer be dismissed as a purely technical issue or a concern reserved for IT departments. One breach is enough to expose the personal data of millions, shake financial markets, and erode the trust between a company and its customers. But beyond the corporate boardrooms and security operation centers, there is a deeper, more human layer to every cyberattack  and it’s unfolding online, in real time. 


### A Look Inside the Noise: Reddit as a Mirror of Cyber Perception 

While news headlines often spotlight big attacks and corporate responses, platforms like **Reddit** offer a bottom up perspective,  revealing what people actually say, feel, and fear when facing digital threats. 

By analyzing thousands of Reddit comments and posts mentioning terms like phishing, data breach, ransomware, or zero trust, a more complex picture emerges. Conversations aren’t always polarized; users express both **concern and confusion**, sometimes anger, sometimes surprise. And the **volume of posts is growing**, suggesting that cybersecurity is no longer a niche topic but it's becoming a **mainstream, lived experience**, especially for those who've had their identities stolen or accounts compromised. 

This growing discourse, rich in emotion and nuance, underscores a simple truth: **cybersecurity is not just about systems, it’s about people**. 

<div style="display: flex; justify-content: center;">
  <div>
    <vegachart
      schema-url="{{ "/assets/charts/intro/emotion_distribution_reddit_dropdown.json" | relative_url }}"
      style="width: 100%; height: 100%"
      tooltip="true" >
    </vegachart>
  </div>
</div>

### What the Emotions Reveal 

As shown in our **emotion analysis** (see technical insight), most users express **negative emotions** — fear, anger, frustration — when discussing cyber incidents. However, there are also traces of relief, curiosity, even humor, proving that digital threats are woven into the emotional fabric of online life. 

These aren’t just isolated incidents; they are a reflection of how modern society processes risk, privacy, and trust in the digital age. 

### Our Approach: Beyond Firewalls and Forensics 

In light of this, our project adopts a **systematic, graph-based approach** to cyber threat intelligence — one that acknowledges not just the technical structure of attacks, but also their social and economic dimensions. 

From **data and maps** to **media coverage, public sentiment, company responses, investment flows, and technical knowledge**, this investigation aims to decode the full lifecycle of cyber threats, with a particular focus on **Italy**. 

<div class="text-center my-3">
  <a href="javascript:void(0)"
     data-bs-toggle="modal"
     data-bs-target="#exampleModal2"
     class="modal-link">
    🛠 <span class="modal_link">Emotion Analysis</span>
  </a>
</div>

<div class="modal fade" id="exampleModal" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
  <div class="modal-dialog modal-xl modal-dialog-centered">
    <div class="modal-content">
      <div class="modal-header">
        <h5 class="modal-title" id="exampleModalLabel">Emotion Analysis</h5>
        <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Chiudi"></button>
      </div>
      <div class="modal-body">
We used the multilingual GordonAI emotion detection model to analyze emotional responses in Reddit posts related to cybersecurity incidents. GordonAI is based on Microsoft’s mdeberta-v3-base and fine-tuned to classify text into seven core emotions: joy, sadness, fear, anger, surprise, disgust, and neutral. It supports English, Italian, and Spanish, and is optimized for short, user-generated texts. 

For this task, we scraped Reddit  title,posts and comments and filtering relavant contents using a curated list of cybersecurity related tokens such as ransomware, phishing, vpn, ddos, exploit, leak, password  and key phrases like "got hacked", "account stolen", "lost access", or "social engineering". 

Each extracted post was processed by the model to detect its dominant emotional tone. This allowed us to explore how users react emotionally to specific threat types, and how different scenarios (e.g., personal account loss vs. general vulnerability disclosure) trigger distinct affective responses. 
      </div>
      <div class="modal-footer">
        <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Chiudi</button>
      </div>
    </div>
  </div>
</div>






# Map the Attack {#map-the-attack}

<div style="display: flex; justify-content: center;">
  <div>
    <vegachart
      schema-url="{{ "/assets/charts/map_the_attack/trend_black.json" | relative_url }}"
      style="width: 100%; height: 100%" 
      tooltip="true" >
    </vegachart>
  </div>
</div>

Since 2020, the world has witnessed a sharp rise in cyberattacks, marking a clear upward trend that shows no sign of slowing down. This phenomenon spans across all continents, with North America experiencing the most pronounced growth, though it's worth noting that the dataset we analyzed is mostly U.S.based, which may partly explain the spike. Europe follows closely, highlighting the global scale of the threat and reinforcing the importance of a focused regional analysis. This escalation is closely linked to the rapid digital transformation triggered by the [COVID-19 pandemic](https://www.eurofound.europa.eu/en/covid-19-and-digitalisation), which compelled organizations, institutions, and individuals to adopt digital technologies at an unprecedented pace, often without adequate cybersecurity safeguards, accelerating digital adoption by three to four years in many sectors. As we shift our focus to comparing trends within Europe, and specifically between Italy and the broader region, this context becomes especially relevant.   


<div class="text-center my-3">
  <a href="javascript:void(0)"
     data-bs-toggle="modal"
     data-bs-target="#exampleModal7"
     class="modal-link">
    🔎 <span class="modal_link">Data Collection and Cleaning</span>
  </a>
</div>

<div class="modal fade" id="exampleModal7" tabindex="-1" aria-labelledby="exampleModal7Label" aria-hidden="true">
  <div class="modal-dialog modal-xl modal-dialog-centered">
    <div class="modal-content">
      <div class="modal-header">
        <h5 class="modal-title" id="exampleModal7Label">Data Collection and Cleaning</h5>
        <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Chiudi"></button>
      </div>
      <div class="modal-body">
For our project, we relied on two different datasets. The first, curated by the <strong>University of Maryland</strong>, spans approximately ten years (from 2014 to mid-2024). The second dataset, obtained from <strong>Ransomfeed</strong>, is more recent, containing some records from mid-2025. These datasets provided complementary perspectives: the Maryland dataset was rich in features such as event_type (e.g., exploitative or disruptive), attack_type (e.g., criminal or hacktivist), as well as detailed descriptions of the attacks and, where available, information about the actors behind them. In contrast, the Ransomfeed dataset had a more structured format, including the following fields: VICTIM, GANG, DATE, YEAR, COUNTRY. It's important to note that both datasets contained **incomplete records** — in many cases, crucial information such as the attacker’s identity or the country targeted was missing. This posed a challenge for analysis, but it reflects the reality that information on cyberattacks is not always publicly available or up to date. 

To work with these datasets, we first performed data cleaning and removed duplicates, which we identified after merging them.  

For what concerns duplicates removal, since we could not check tens of thousands of records manually, we did this check with the help of fuzzy matching: we compared pairs of records from the two different datasets belonging to the same year, and we computed the fuzzy matching score of the respective organizations. If this score was above a given threshold, than the organizations could be the same (although their names actually differed), and so we validated them manually. Doing this automatic prefiltering with fuzzy matching allowed us to dramatically speedup the process of data deduplication. 

Next, we enriched the data: for each record, we used the attack’s country to classify it by continent, enabling us to analyze geographical trends. We also added geographic coordinates (latitude and longitude) for each country using a JSON file sourced online. 

For attacks targeting Italian organizations specifically, we went further: we manually identified the headquarters of each affected company and retrieved their coordinates using publicly available sources. This allowed us to generate a detailed map of cyberattacks in Italy using <strong>Folium</strong> and to create heatmaps of attack density within Italy using Altair. The rest of the visualizations in our analysis were also produced with <strong>Altair</strong>  
      </div>
      <div class="modal-footer">
        <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Chiudi</button>
      </div>
    </div>
  </div>
</div>



<div style="display: flex; justify-content: center; align-items: center; gap: 20px; width: 100%;">
  <div style="flex: 0 0 50%;">
    <vegachart
      schema-url="{{ "/assets/charts/map_the_attack/rank_italy_attack_count_black.json" | relative_url }}"
      style="width: 100%; height: 100%;" 
      tooltip="true">
    </vegachart>
  </div>

  <div style="flex: 0 0 50%; display: flex; align-items: center;">
    <vegachart
      schema-url="{{ "/assets/charts/map_the_attack/cloropleth_blu_verde_black.json" | relative_url }}"
      style="width: 100%; height: auto;" 
      tooltip="true">
    </vegachart>
  </div>
</div>


Following this overview, our data identified Italy as the second most targeted country in Europe, with around **900 attacks**, trailing only the United Kingdom, which recorded approximately 1,500. The gap is significant, yet **Italy** clearly remains a **primary target**. Other major European powers like France, Germany, Spain, and Russia also rank among the top, though they fall behind Italy in total incidents. On a global scale, Italy still holds a prominent position, ranking **fourth** overall (after USA, UK and Canada). The United States dominates the landscape with a dramatically higher volume of attacks, underscoring both the scale of the threat and the importance of regional resilience.


<div style="display: flex; justify-content: center;">
  <div>
    <vegachart
      schema-url="{{ "/assets/charts/map_the_attack/average_trend_italy_europe_black.json" | relative_url }}"
      style="width: 100%; height: 100%" 
      tooltip="true" >
    </vegachart>
  </div>
</div>


When comparing Italy’s cyber-attack trend to the European average, a clear divergence emerges. In certain years, such as **2017** or **2020**, the numbers were nearly aligned, suggesting a **comparable threat level**. But shortly thereafter, Italy's curve began to **rise** steadily, with **sharp peaks starting around 2021**. This contrasts sharply with the broader European trend, which has remained comparatively moderate. This gap highlights the urgent **need for focused attention on Italy**, where cyber threats are escalating at a faster pace, calling for targeted, localized analysis and response. The plot depicting this comparison uses Italian cyber-attack data alongside a population-weighted European average, calculated using 2024 population figures per country to provide a more accurate regional context. 

This brings us to the core of our investigation: **who is being targeted the most in Italy and why**? To better understand this phenomenon, it's essential to first clarify the structure of the Italian corporate landscape. The characteristics of the national business ecosystem play a key role in shaping both the exposure and vulnerability of different actors. The overview below provides a snapshot of this landscape, setting the stage for a deeper analysis of attack patterns and motivations.


![Infografica]({{ "/assets/images/infografica.png" | relative_url }})

The infographic is based on data from **ISTAT (2022)**, not the most recent, but still a reliable reference for outlining the structure of Italian enterprises. According to this data, Italy hosts a large number of businesses, the vast majority of which are **micro** and **small enterprises**, making up **78.9%** and **18.5%** of the total, respectively. This small-scale composition has important implications for cybersecurity readiness and resilience. In terms of geographic distribution, there is a clear regional divide: the North of Italy dominates; specifically, the **North-West** accounts for **28.7%** of these businesses, while the **North-East** follows with **22.7%**. 


This foundational overview helps contextualize **which types of organizations are more exposed to cyber threats and why**. Understanding Italy’s business landscape is essential not only for assessing organizational readiness, but also for interpreting where and how cyberattacks unfold. Building on this, we turned our attention to the **geographic distribution** of attacks, examining not just their frequency, but how they align with the economic and structural profiles of each region. 


<div class="hm-buttons">
  <button type="button" class="hm-btn1 active" data-target="heatmap1">Attacks per Region</button>
  <button type="button" class="hm-btn1" data-target="heatmap2">Attacks / Revenue</button>
  <button type="button" class="hm-btn1" data-target="heatmap3">Attacks / Companies</button>
</div>

<div id="heatmap1" class="heatmap visible">
  <div>
    <vegachart
      schema-url="{{ "/assets/charts/heatmap1.json" | relative_url }}"
      style="width: 100%; height: 100%" 
      tooltip="true" >
    </vegachart>
  </div>
</div>

<div id="heatmap2" class="heatmap">
  <div>
    <vegachart
      schema-url="{{ "/assets/charts/heatmap2.json" | relative_url }}"
      style="width: 100%; height: 100%" 
      tooltip="true" >
    </vegachart>
  </div>
</div>

<div id="heatmap3" class="heatmap">
  <div>
    <vegachart
      schema-url="{{ "/assets/charts/heatmap3.json" | relative_url }}"
      style="width: 100%; height: 100%" 
      tooltip="true" >
    </vegachart>
  </div>
</div>


When examining the distribution of attacks across Italian regions, both in terms of raw incident counts and data normalized by the number of companies and total regional revenue, **Lombardy** unsurprisingly emerges as the most targeted region, followed by **Lazio**. Overall, cyberattacks appear more concentrated in **Northern Italy**, a trend aligned with ISTAT data showing that **over 50%** of Italian companies are based in the North. However, Lazio still stands out. Even when adjusting for business density, it ranks among the most attacked regions, likely due to the concentration of **public administration institutions in Rome**, which might represent a target for **ideologically motivated** threat actors.

**Italy ranks among the lowest in Europe for digital skills**: according to the Digital Economy and Society Index ([DESI](https://digital-strategy.ec.europa.eu/it/policies/desi)), only **46%** of Italians had at least basic digital skills in 2021, far below the EU average and well behind countries like the Netherlands and Finland (both at 79%). **This digital gap is particularly pronounced in Southern Italy**, often perceived as more vulnerable to cyber threats due to lower levels of digital readiness. 

When attacks are normalized by regional revenue, **Lazio** remains prominent, alongside wealthy industrial regions like Lombardy, Piedmont, and Emilia-Romagna. Interestingly, several Southern and Central regions, such as Campania, Umbria, and Molise, also appear disproportionately targeted. This may reflect the presence of high-revenue enterprises within otherwise smaller business ecosystems, making them attractive targets for **financially motivated threat actors**. Overall, the distribution underscores that cybercriminals tend to prioritize **economic value** and **digital surface area**, rather than focusing solely on raw company numbers or regions perceived as less prepared.


### Zooming in: Cyberattacks across Italy, one incident at a time


Beyond the numbers and trends, each cyberattack tells a story, of **disruption, vulnerability, and intent**. This map brings those stories into focus, marking the real-world locations where digital threats have struck Italian organizations. From ransomware assaults on manufacturing firms in Lombardy to breaches in public institutions across Lazio, the geography of cyber risk mirrors the country’s economic and institutional footprint. Some regions emerge as **hot spots**; others reveal isolated but high-impact incidents, each one leaving behind a trail of consequences, some still unfolding. This view reminds us that **cybersecurity is not just a systemic issue, it’s a local one, too**. Behind every point on the map is a breach that mattered.


<div> 
  <iframe src="{{ site.baseurl }}/assets/charts/map_the_attack/mappa_italia_aziende_hq_description.html" width="100%" height="400px" frameborder="0"></iframe> 
</div>

<br><br><br>
When analyzing the Italian dataset more deeply, a recurring pattern emerges: the most targeted sector is **Manufacturing**, followed by **Public Administration**. 

Sector-specific data confirms these vulnerabilities: in 2023, the manufacturing sector accounted for **13% of all cyberattacks in Italy, more than twice its global share** ([Muscope report](https://www.muscope.com/en/industry-manufacturing/?utm_source=chatgpt.com)). This makes it a clear target for ransomware groups and threat actors aiming to disrupt production or exfiltrate valuable data. A complementary perspective based on **organization size** reinforces this narrative: SMEs account for **more than 400 attacks**, representing **over half of all recorded incidents**. This aligns with ISTAT data showing that SMEs make up the overwhelming majority of Italian businesses. Public Administration, the second most attacked sector, also ranks high by size category. 




<div class="hm-buttons">
  <button type="button" class="hm-btn2 active" data-target="barchart1">Attacks by Sector</button>
  <button type="button" class="hm-btn2" data-target="barchart2">Attacks by Company Type</button>
</div>

<div id="barchart1" class="barchart visible">
  <div>
    <vegachart
      schema-url="{{ "/assets/charts/map_the_attack/industry_size_italy_black.json" | relative_url }}"
      style="width: 100%; height: 100%" 
      tooltip="true" >
    </vegachart>
  </div>
</div>


<div id="barchart2" class="barchart">
  <div>
    <vegachart
      schema-url="{{ "/assets/charts/map_the_attack/SETTORI_COLPITI_ITALY_BLACK.json" | relative_url }}"
      style="width: 100%; height: 100%" 
      tooltip="true" >
    </vegachart>
  </div>
</div>


This trend is tied to both **economic weight and accelerated digitalization**, especially among small and medium enterprises (SMEs), which often lack robust cybersecurity practices. According to the [Cyber Index PMI 2024](https://www.confindustria.it/progetti/cyber-index-pmi/) by Confindustria, Politecnico di Milano, and the Italian National Cybersecurity Agency, Italian SMEs score an average of just **52 out of 100** in terms of **cyber resilience**. At the European level, [ENISA](https://www.enisa.europa.eu/topics/awareness-and-cyber-hygiene/smes-cybersecurity) also reports that **over 90% of SMEs** adopted digital tools during the pandemic **without strengthening their cybersecurity posture**, leaving many exposed to exploitive threats.

While Italy does not rank among the most digitally advanced countries in the EU, its position as one of the most frequently targeted by cyberattacks may, paradoxically, stem from that very imbalance. As one cybersecurity expert we interviewed explained:
> _If all intrusions were actually detected and publicly reported, Italy would likely top the European charts._

According to this perspective, Italy’s vulnerability lies not only in the number of connected systems, but in how **unprepared** many institutions are to secure them. Three core factors were cited. First, there’s a widespread **lack of cybersecurity expertise at the decision-making level**, both within companies and in the public bodies meant to protect them. Cybersecurity governance is often assigned to professionals with legal or administrative backgrounds, who may lack the technical expertise required to keep pace with fast-evolving digital threats. Second, **security** is still widely **perceived as a cost rather than a strategic investment**, a cultural mindset that ultimately **discourages proactive defense**. Lastly, the Italian cybersecurity market is dominated by few large enterprises with ties to the defense sector, whose priorities are often misaligned with the needs of Italy’s industrial backbone (small and medium enterprises). This leads to a slow and uncoordinated response system, **leaving much of Italy’s digital infrastructure vulnerable to attacks**.

Together, these findings reflect a broader trend: **cybercriminals prioritize sectors where disruption is most impactful, and defenses are uneven**. This raises a critical question: **are certain threat actors consistently targeting specific industries in Italy and if so, why?** The answer can reveal strategic intent, ranging from financial motives to ideological agendas, and help prevent future risks. 

The following section explores this dynamic in greater detail, examining how **key threat actors operate in Italy** and which industries they pursue most aggressively.

<div style="display: flex; justify-content: center;">
  <div>
    <vegachart
      schema-url="{{ "/assets/charts/map_the_attack/HEATMAP_ACTOR_INDUSTRY_BASTA_VERAMENTE_BLACK.json" | relative_url }}"
      style="width: 100%; height: 100%" 
      tooltip="true" >
    </vegachart>
  </div>
</div>



<div class="text-center my-3">
  <a href="javascript:void(0)"
     data-bs-toggle="modal"
     data-bs-target="#exampleModal5"
     class="modal-link">
    👾 <span class="modal_link">Actors Overview</span>
  </a>
</div>

<div class="modal fade" id="exampleModal5" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
  <div class="modal-dialog modal-xl modal-dialog-centered">
    <div class="modal-content">
      <div class="modal-header">
        <h5 class="modal-title" id="exampleModalLabel">Actors Overview</h5>
        <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Chiudi"></button>
      </div>
      <div class="modal-body">

        <section>
          <h5>LockBit 3.0</h5>
          <p>One of the most advanced and active ransomware-as-a-service (RaaS) groups globally. It emerged as a rebrand of previous LockBit versions, introducing technical upgrades and a unique bug bounty program to reward vulnerability reports. Responsible for over 2,000 victims and more than $120 million in ransom payments, LockBit 3.0 is known for its aggressive double-extortion tactics and high success rate.</p>
        </section>

        <section>
          <h5>LockBit 2.0</h5>
          <p>The second major version in the LockBit lineage, active throughout 2021 and early 2022. It refined encryption speeds, expanded affiliate operations, and popularized double extortion and leak site usage. It laid the groundwork for the more advanced LockBit 3.0.</p>
        </section>

        <section>
          <h5>Akira</h5>
          <p>A RaaS group that surfaced in 2023, likely involving former Conti affiliates. Known for targeting both Windows and Linux environments using custom-built encryptors. Akira often gains access via compromised VPN credentials and communicates with victims in a casual, even mocking tone on its leak site.</p>
        </section>

        <section>
          <h5>8Base</h5>
          <p>Emerging in 2022, 8Base uses double-extortion tactics and custom ransomware that avoids encrypting certain file types to keep systems partially operational. The group relies on affiliates and has been disrupted by international law enforcement actions, though it remains active.</p>
        </section>

        <section>
          <h5>Conti</h5>
          <p>Once among the most feared RaaS groups, Conti operated like a professional corporation, complete with internal training, salaries, and bonuses. It attacked over 700 victims using high-quality ransomware and cultivated skilled affiliates. Leaked documents suggest ambitions beyond ransomware, including crypto exchanges and dark web platforms.</p>
        </section>

        <section>
          <h5>BlackBasta</h5>
          <p>Appeared in 2022, likely as a Conti/BlackMatter offshoot. The group quickly gained notoriety with large-scale attacks, including against Synlab Italia. It employs fast deployment, double extortion, and steep ransom demands.</p>
        </section>

        <section>
          <h5>Alphv</h5>
          <p>First observed in 2021 and written entirely in Rust, Alphv is run by Russian-speaking actors linked to DarkSide and BlackMatter. Its RaaS model offers affiliates generous revenue shares and supports highly customizable attacks, including triple extortion (encryption, data theft, DDoS).</p>
        </section>

        <section>
          <h5>Cactus</h5>
          <p>A newer ransomware group, active since late 2023, primarily targeting Italian organizations. It uses selective encryption and double-extortion tactics. Known for its aggressive negotiation approach and growing technical sophistication.</p>
        </section>

        <section>
          <h5>RansomHub</h5>
          <p>An emerging RaaS group since early 2024, known for targeting critical sectors like healthcare and finance. It quickly exploits known vulnerabilities and works with experienced affiliates. After a brief disappearance in 2025, it has resumed operations.</p>
        </section>

        <section>
          <h5>NoEscape</h5>
          <p>Appeared in 2023, likely as a reboot of the defunct Avaddon group. Offers affiliates a full-featured attack panel and uses multi-extortion tactics, including threats of data leaks and public exposure.</p>
        </section>

        <section>
          <h5>Rhysida</h5>
          <p>Launched in May 2023 and presenting itself as a “cybersecurity team,” Rhysida uses phishing to gain access, followed by double extortion. It has attacked government, healthcare, and educational institutions, including the British Library.</p>
        </section>

        <section>
          <h5>Medusa</h5>
          <p>A fast-rising RaaS group since 2023, initially closed but now affiliate-based. Uses phishing and double extortion, with public promotion of attacks via Telegram and social media. Known victims include Toyota Financial Services and the Minneapolis School District.</p>
        </section>

        <section>
          <h5>Malas</h5>
          <p>Emerging in March 2023, MalasLocker is ideologically driven, demanding donations to approved charities instead of ransom payments. It targets Zimbra servers via phishing and exploits and has attacked sectors in countries like Italy, Russia, and the U.S.</p>
        </section>

        <section>
          <h5>Noname057(16)</h5>
          <p>A pro-Russian hacktivist group active since March 2022. It conducts large-scale DDoS attacks against Western targets, including government and media websites, often using the open-source tool “DDoSIA” to coordinate volunteer participants. Despite a major takedown effort in 2024, it remains active and aligned with other hacktivist groups.</p>
        </section>

        <section>
          <h5>Lulzsecita</h5>
          <p>An Italian hacktivist cell linked to the global LulzSec collective, most active in the mid-2010s. Known for using SQL injection attacks against Italian universities and public entities to expose vulnerabilities and make political statements.</p>
        </section>

      </div>
      <div class="modal-footer">
        <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Chiudi</button>
      </div>
    </div>
  </div>
</div>





The data highlights how different sectors are targeted in different ways. **LockBit 3.0** is the most active and geographically distributed group, with a distinct preference for **Manufacturing**, echoing the earlier finding that this sector is the most targeted. Its predecessor, **LockBit 2**, displayed a broader distribution, with a notable presence in **Retail** and **General Services**, but less strategic focus overall. By contrast, politically motivated actors like **Noname057(16)** and **LulzSecITA** mainly targeted **Public Administration**, largely bypassing manufacturing. This suggests a goal not of profit but of visibility, through public disruption or data leaks, exploiting institutional vulnerabilities.

A look at timelines further illustrates these dynamics. As of June 2025, only a few groups, **Akira, Cactus, Rhysida, 8Base**, and **Lockbit 3.0**, remain active in Italy, reflecting a possible shift in ransomware models. Meanwhile, **LulzSecITA**’s campaigns ended by 2020, and **LockBit 3.0** appears to have seamlessly replaced **LockBit 2**, suggesting operational continuity. The first LockBit 3.0 attacks followed immediately after LockBit 2 ceased operations, indicating **rebranding**, not retirement.

<div style="display: flex; justify-content: center;">
  <div>
    <vegachart
      schema-url="{{ "/assets/charts/map_the_attack/duration_gangs_italy_ok_prova1_black.json" | relative_url }}"
      style="width: 100%; height: 100%" 
      tooltip="true" >
    </vegachart>
  </div>
</div>


Another layer of analysis explored whether these actors are **Italy-specific** or operate across Europe. The answer is nearly unanimous: 14 out of the top 15 actors active in Italy also conduct campaigns throughout Europe. The only exception is **Sandworm**, a Russian state-sponsored group known for critical infrastructure attacks. Its absence in Italy likely reflects a strategic focus on more geopolitically sensitive targets elsewhere in Europe ([MITRE ATT&CK](https://attack.mitre.org/groups/G0034/)). 

<div style="display: flex; justify-content: center;">
  <div>
    <vegachart
      schema-url="{{ "/assets/charts/map_the_attack/attori_europa_black.json" | relative_url }}"
      style="width: 100%; height: 100%" 
      tooltip="true" >
    </vegachart>
  </div>
</div>



<div class="text-center my-3">
  <a href="javascript:void(0)"
     data-bs-toggle="modal"
     data-bs-target="#exampleModal6"
     class="modal-link">
    👾 <span class="modal_link">Actor Overview</span>
  </a>
</div>

<div class="modal fade" id="exampleModal6" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
  <div class="modal-dialog modal-xl modal-dialog-centered">
    <div class="modal-content">
      <div class="modal-header">
        <h5 class="modal-title" id="exampleModalLabel">Actor Overview</h5>
        <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Chiudi"></button>
      </div>
      <div class="modal-body">

        <section>
          <h5>Sandworm (Unit 74455)</h5>
          <p>A state-sponsored Russian cyber warfare group under the GRU, infamous for large-scale disruptive attacks like NotPetya and Industroyer2. Specializes in sabotage of critical infrastructure across Ukraine, Europe, and NATO countries. </p>
        </section>

      </div>
      <div class="modal-footer">
        <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Chiudi</button>
      </div>
    </div>
  </div>
</div>




To conclude our exploration of cyber actor dynamics, we conducted a **clustering analysis of behavioral patterns and target preferences**. This yielded **10 distinct groups**, all showing intense activity in **Lombardy**, Italy’s economic engine, and in **Lazio**, specifically cluster 2 and 8, a region rich in institutional targets. **Cluster 3** stands out for its exclusive **focus on Veneto**, perhaps drawn by local industry or regional vulnerabilities. Overall, the clustering confirms that **regional economics**, especially those with dense concentrations of SMEs and public assets, remain priority targets for cyber threat actors.

![Cluster]({{ "/assets/images/regions_actors_company_type_cluster.png" | relative_url }})


<div class="text-center my-3">
  <a href="javascript:void(0)"
     data-bs-toggle="modal"
     data-bs-target="#exampleModal8"
     class="modal-link">
    🛠️ <span class="modal_link">Clustering</span>
  </a>
</div>

<div class="modal fade" id="exampleModal8" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
  <div class="modal-dialog modal-xl modal-dialog-centered">
    <div class="modal-content">
      <div class="modal-header">
        <h5 class="modal-title" id="exampleModalLabel">Clustering</h5>
        <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Chiudi"></button>
      </div>
      <div class="modal-body">

        <section>
          <p>We conducted a clustering analysis to group threat actors based on their behavioral patterns, using two key categorical features: geographical region and targeted company type. 

          The dataset was preprocessed and encoded appropriately for clustering. We applied K-Means clustering to identify groups of actors with similar targeting behaviors. To determine the optimal number of clusters (K), we used the Elbow Method. This was further validated using Silhouette Scores to assess the cohesion and separation of clusters. </p>

          <div class="d-flex justify-content-center gap-3 flex-wrap mt-4">
            <img src="{{ '/assets/images/elbow_method.png' | relative_url }}" alt="Elbow Plot" class="img-fluid" style="max-width: 48%;">
            <img src="{{ '/assets/images/silhouette.png' | relative_url }}" alt="Silhouette Plot" class="img-fluid" style="max-width: 48%;">
          </div>

          <p>Both methods indicated that an optimal number of clusters lies around K = 10, balancing model complexity with interpretability. This clustering serves as a foundational step for profiling actor groups and analyzing their targeting trends more effectively.  

          Thanks to this process, we were able to identify a distinct behavioral pattern in Cluster 3, which appears to focus on the Veneto region. Further details about its composition are provided in the figures below.  </p>

          <div class="d-flex justify-content-center gap-3 flex-wrap mt-4">
            <img src="{{ '/assets/images/img1.jpeg' | relative_url }}" alt="Immagine 1" class="img-fluid" style="max-width: 32%;">
            <img src="{{ '/assets/images/img2.jpeg' | relative_url }}" alt="Immagine 2" class="img-fluid" style="max-width: 32%;">
            <img src="{{ '/assets/images/img3.jpeg' | relative_url }}" alt="Immagine 3" class="img-fluid" style="max-width: 32%;">
          </div>

        </section>

      </div>
      <div class="modal-footer">
        <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Chiudi</button>
      </div>
    </div>
  </div>
</div>


### From Breach to Awareness: Is the Threat Truly Understood?


This deep dive into sectoral and regional patterns confirms a fundamental truth: **Italy’s most productive and institutional regions are at the center of its cyber threat landscape**. Whether due to economic weight, critical data exposure, or structural weaknesses, these areas face elevated and persistent risks. But here’s the real question: **does the public understand the scale of this threat?** In an age where ransomware can stop hospitals from working, leak court information, or shut down factories, one would expect cyberattacks to dominate headlines and shape national policy conversations. And yet, **visibility doesn't always match severity**. The next section shifts focus from the attackers to the **narrative**, how cyber incidents are portrayed in Italian media, acknowledged by institutions, and ultimately **perceived by society**. 

<br><br><br>


# Breaking the Net {#breaking-the-net}

### When Cyberattacks Happen, Who's Listening?

<div style="display: flex; justify-content: center;">
  <div>
    <vegachart
      schema-url="{{ "/assets/charts/breaking_the_net/1_aziende/sentiment_by_source_origin_chart.json" | relative_url }}"
      style="width: 100%; height: 100%"
      tooltip="true" >
    </vegachart>
  </div>
</div>

Now that we’ve examined who is being targeted by cyberattacks in Italy, who the threat actors are, and the techniques they use, we can turn to an equally important question: how are these incidents portrayed in the public sphere? 

From 2015 to 2025, there have been around 900 documented cyberattacks on Italian companies. But, as this graph shows, only 118 of those were actually mentioned in the media. Each dot represents a cyberattack, and only the blue ones were covered in news outlets, while the red ones received no media attention at all. 

We can clearly see a growing number of attacks over time, especially after 2020. Yet the gap between attacks and media coverage remains wide. This tells us that despite the rising frequency and impact of cyber incidents, the Italian media only reports a small fraction of them. This underrepresentation could have serious implications for public awareness, corporate accountability, and national cybersecurity policy. 


### Niche Networks, National Silence   

<div style="display: flex; justify-content: center;">
  <div>
    <vegachart
      schema-url="{{ "/assets/charts/breaking_the_net/1_aziende/2.articles_by_source_type.json" | relative_url }}"
      style="width: 100%; height: 100%"
      tooltip="true" >
    </vegachart>
  </div>
</div>

Furthermore, if we dig deeper into the few cases that were covered by the media, another pattern emerges. Most of these reports come from cybersecurity-focused outlets — specialized industry publications that primarily reach a niche audience of professionals and insiders. 

This means that the general public, who typically relies on mainstream newspapers and national media, is **often left unaware of these incidents**. As a result, communication around cyber threats in Italy remains limited and fragmented. The lack of broader media coverage contributes to a low level of public awareness and understanding of cybersecurity risks, despite their growing relevance in everyday life and business. 

So, while attacks are increasing in both frequency and severity, the information about them struggles to reach the wider population, weakening Italy's collective ability to respond, prepare, and build a stronger cybersecurity culture. 

### Which Sectors Make the Headlines? 

<div style="display: flex; justify-content: center;">
  <div>
    <vegachart
      schema-url="{{ "/assets/charts/breaking_the_net/1_aziende/sentiment_by_industry_chart.json" | relative_url }}"
      style="width: 100%; height: 100%"
      tooltip="true" >
    </vegachart>
  </div>
</div>

<div style="display: flex; justify-content: center;">
  <div>
    <vegachart
      schema-url="{{ "/assets/charts/breaking_the_net/1_aziende/normalized_chart.json" | relative_url }}"
      style="width: 100%; height: 100%"
      tooltip="true" >
    </vegachart>
  </div>
</div>

After this general overview, we can now reflect on the types of industries affected by cyberattacks and the sentiment of media coverage. 

In the first graph, which shows the average number of articles per attack, we see that **utilities** such as electricity, water, or gas providers receive the **highest media coverage per attack**, even though they were only targeted three times. This indicates a strong media focus on critical infrastructure, likely due to the potential impact on public life and national security. 

In the second graph, which breaks down the **sentiment of articles by industry**, utilities again stand out with a high **share of negative sentiment**. This could be due to an alarmist tone often used when essential services are disrupted, emphasizing risk and urgency. 

However, if we look at **sectors that were less frequently attacked**, such as **transportation and warehousing, accommodation and food services, or mining and extraction**, we notice that these receive **little to no negative coverage**. In some cases, the sentiment is even neutral or slightly positive. This may be because these incidents are seen as less critical or less interesting for the general audience, and therefore are reported with a softer tone or not at all. 

This contrast highlights how **media visibility and tone are not only tied to the frequency of attacks**, but also to how **newsworthy or alarming** an incident is perceived to be. 


###  Cybersecurity: What We Say, What We Mean 

<div style="display: flex; justify-content: center;">
  <div>
    <vegachart
      schema-url="{{ "/assets/charts/breaking_the_net/2_comparative/NEW_most_frequent_tokens_by_source.json" | relative_url }}"
      style="width: 100%; height: 100%"
      tooltip="true" >
    </vegachart>
  </div>
</div>


In cybersecurity, **words matter** and so does the emotional charge we attach to them. While the frequency of keywords such as data breach, malware, or privacy may be similar across different sources, the **emotions and tones surrounding them are not**. 

  
Our sentiment analysis reveals a striking pattern: **regardless of the source**, cybersecurity-related language tends to carry a **negative connotation**. However, something begins to shift starting in **2020**. 



<div style="display: flex; justify-content: center;">
  <div>
    <vegachart
      schema-url="{{ "/assets/charts/breaking_the_net/2_comparative/2.sentiment_giornali_settore_2017_2024.json" | relative_url }}"
      style="width: 100%; height: 100%"
      tooltip="true" >
    </vegachart>
  </div>
</div>

Even within general news media, we observe a **gradual trend toward more neutral — and occasionally positive — tones**, particularly when coverage involves **governmental initiatives** or **platforms responding to attacks**. 


<div style="display: flex; justify-content: center;">
  <div>
    <vegachart
      schema-url="{{ "/assets/charts/breaking_the_net/2_comparative/3.top_entities_sentiment_by_source.json" | relative_url }}"
      style="width: 100%; height: 100%"
      tooltip="true" >
    </vegachart>
  </div>
</div>

By contrast, sector-specific sources maintain a more **technical register**, focusing on topics such as GDPR compliance, enterprise protection strategies, and the role of **DPOs (Data Protection Officers)**. The same words — security, threat, vulnerability — are used, but the **associated sentiment changes** dramatically depending on the source. 

This divergence is key. 

###  When Optimism Stays in the Echo Chamber 

What do we really talk about when we talk about cybersecurity? 

By measuring the average sentiment across dominant topics and sources, a striking pattern emerges: **positive tones are almost exclusively reserved for sector-specific publications**, and only when discussing **corporate security and legal compliance**. These include discussions on enterprise level risk management, GDPR enforcement, and organizational resilience themes treated with a sense of control, even optimism. 

Everywhere else, the tone shifts. 

In mainstream journalism, where the audience is broader and less specialized, **the sentiment trends negative  across the board**. Stories around personal privacy, digital fraud, or user tracking are overwhelmingly framed in critical terms, with few signs of hope or solutions. The most negative tones appear when users and their devices are at the center of the narrative. 

The contrast is even sharper when the same topic is handled by different sources. For example, corporate cybersecurity is portrayed by industry media as an evolving opportunity a space of innovation and strategic growth. But in the general press, it’s nearly absent unless tied to crisis, scandal, or systemic failure. 


**Clustering analysis  also reveals a fragmented cyber discourse.** Sector-specific publications tend to focus on regulatory compliance and enterprise risk, usually adopting a neutral or critical tone  except in 2024, when optimism emerges around corporate cybersecurity success stories. In contrast, general media emphasizes personal privacy and cybercrime, often with emotional and negative framing, especially during crises like the pandemic. 

Notably, the only positive sentiment cluster originates from the sector  suggesting that optimism is largely internal and professional. Even shared topics, like corporate cybersecurity, are portrayed very differently: as progress in the sector, and as crisis in the public media narrative. 

 
This divergence reveals more than just editorial choices: it points to a **split in how cybersecurity is understood, communicated, and emotionally processed**, depending on who’s talking and who’s listening. 

In short, **confidence lives in the sector. Concern dominates the public sphere**. 

And that divide might be exactly what’s preventing Italy from building a truly shared cyber resilience culture. 



### A Communication Gap That Shapes Action 

This gap isn’t just semantic, it’s strategic. 

 If the **perception of cybersecurity** remains focused solely on breaches and blame, while technical sources highlight regulation, governance, and risk management, the broader public may fail to grasp the full scope of what's at stake. 

This discrepancy is confirmed by recent research. 

According to the **Cyber Index PMI 2024**, only **15%** of Italian small and medium enterprises have a strategic approach to cyber risk. **Over half (56%) still lack awareness or tools to react effectively**. The disconnect is not just about capacity , it’s about narrative. If risk is not communicated with clarity and realism, action will lag behind awareness. 

A 2024 cross-cultural study further supports this view: 

While Italians acknowledge cyber threats as real, they tend to adopt a **passive, delegated approach**, trusting institutions or service providers to take care of security. Compared to countries like Germany or the UK, Italy stands in the middle tier: aware, but not proactive.([paper](https://arxiv.org/abs/2405.16215v2)) 

### A Final Call: Words Are Not Just Words 

When **cyber language is fragmented**, so is the response. 

From newsrooms to boardrooms, from small and medium enterprises to government agencies, the way we **talk** about cybersecurity shapes the way we **invest, legislate, educate, and defend**. 

The good news? The data shows change is possible. Positive narratives do emerge  especially when **solutions, not just threats**, are placed at the center. But to bridge the communication gap, we need **more than analysis**. We need a **shared language**, one that makes cybersecurity not just a technical domain, but a **collective priority**. 


**TODO** sistema questi grafici

  <div>
    <vegachart
      schema-url="{{ "/assets/charts/breaking_the_net/2_comparative/4.article_clusters_dashboard.json" | relative_url }}"
      style="width: 100%; height: 100%"
      tooltip="true" >
    </vegachart>
  </div>



<div style="display: flex; justify-content: center;">
  <div>
    <vegachart
      schema-url="{{ "/assets/charts/breaking_the_net/1_aziende/media_coverage_cyberattacks.json" | relative_url }}"
      style="width: 100%; height: 100%"
      tooltip="true" >
    </vegachart>
  </div>
</div>


<div style="display: flex; justify-content: center;">
  <div>
    <vegachart
      schema-url="{{ "/assets/charts/breaking_the_net/1_aziende/post_attack_topics_chart.json" | relative_url }}"
      style="width: 100%; height: 100%"
      tooltip="true" >
    </vegachart>
  </div>
</div>







<div style="display: flex; justify-content: center;">
  <div>
    <vegachart
      schema-url="{{ "/assets/charts/breaking_the_net/1_aziende/source_origin_chart.json" | relative_url }}"
      style="width: 100%; height: 100%"
      tooltip="true" >
    </vegachart>
  </div>
</div>




<div class="text-center my-3">
  <a href="javascript:void(0)"
     data-bs-toggle="modal"
     data-bs-target="#exampleModal2"
     class="modal-link">
    🛠 <span class="modal_link">Sentiment Analysis</span>
  </a>
</div>

<div class="modal fade" id="exampleModal2" tabindex="-1" aria-labelledby="exampleModal2Label" aria-hidden="true">
  <div class="modal-dialog modal-xl modal-dialog-centered">
    <div class="modal-content">
      <div class="modal-header">
        <h5 class="modal-title" id="exampleModal2Label">Emotion Analysis</h5>
        <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Chiudi"></button>
      </div>
      <div class="modal-body">
To understand how cybersecurity is discussed we built a custom natural language processing (NLP) pipeline. First, we cleaned and structured the text data using classic yet essential techniques: tokenization, lemmatization, stopword removal and  regular expressions (regex) given the limitations of traditional stopword lists especially when dealing with linguistic contractions, reflexive forms, and informal expressions. Then we moved on to classifying sentiment and identifying underlying themes: 

We used a multilingual transformer model clapAI/modernBERT-large to label every article, post, and comment as positive, neutral, or negative. 

To uncover recurring themes, we applied Latent Dirichlet Allocation (LDA), a probabilistic model that identifies clusters of related words and organizes content around them. 

We tested different numbers of topics (3, 5, 7, 10) using GridSearchCV to find the most informative structure. This process surfaced topics like: Corporate Cybersecurity practices, Data privacy and GDPR, compliance, Cyberattacks and Digital Crime etc.  

Each topic, in turn, was analyzed for sentiment,emotion ( with the model described in the previous technical section) and time allowing us to see not just what was being discussed, but how it evolved across years and media types. 
      </div>
      <div class="modal-footer">
        <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Chiudi</button>
      </div>
    </div>
  </div>
</div>



# Cyber Q&A {#cyber-q-and-a}




###  Shared Knowledge: The Intelligent Graph Bridging Cybersecurity Gaps 

<div> 
  <iframe src="{{ site.baseurl }}/assets/graph/top50_articles_mitre_graph.html" width="100%" height="400px" frameborder="0"></iframe> 
</div>

In cybersecurity, the communication gap is as critical as the technical one. On one side, we have mainstream media amplifying panic around cyber threats. On the other, trade journals speak a language so technical that it alienates most corporate professionals. Stuck in between are companies eager to train staff, yet often ill-equipped to explain the very threats they face. 

To bridge this divide, we’ve developed an intelligent knowledge graph: a dynamic, visual tool that turns complex cyber data into structured, explorable insights. Designed not for the public at large, but for use in corporate training courses, the graph acts as a semantic map of the cybersecurity landscape, supporting workshops, awareness sessions, and post-training engagement. 

Rooted in the MITRE ATT&CK framework and enriched with peer-reviewed research from PubMed, Crossref, and arXiv, the graph hosts over 4,000 nodes connecting attack techniques, malware families, vulnerabilities, countermeasures, and more. Need to understand how a ransomware campaign exploits a specific vulnerability? Or which mitigations align with spear phishing? The graph doesn't just hold that knowledge, it makes it navigable. 

Even more powerfully, the system integrates a local LLM (Mistral 7B) capable of answering natural language queries using context from the graph itself. Ask a question like “Which mitigations are most effective against credential dumping?” and get a grounded, explainable response. Combined with interactive visualizations and slide generation, it becomes a training companion, not just a data tool. 


### The Communication Gap Is Real 

According to the 2° CensisIISFA (2023/2024) Report, 20.8% of Italian workers still don’t know what "cybersecurity" even means — up from 17.1% the year before. Meanwhile, over 1 in 5 employees have witnessed a cybersecurity incident in their workplace in the last year, ranging from service disruptions to data breaches. And yet, much of the training still relies on static materials and vague definitions. 

In this context, tools like our knowledge graph aren’t just useful, they’re necessary. They educate. They contextualize. They make cybersecurity make sense. 


<iframe width="100%" height="400" src="https://www.youtube.com/embed/RI0W7NRl4SU?si=exRRIXoy2hr_qgFb&vq=hd1080" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>




<div class="text-center my-3">
  <a href="javascript:void(0)"
     data-bs-toggle="modal"
     data-bs-target="#exampleModal3"
     class="modal-link">
    🛠 <span class="modal_link">Building a Graph of Cyber Knowledge </span>
  </a>
</div>

<div class="modal fade" id="exampleModal3" tabindex="-1" aria-labelledby="exampleModal3Label" aria-hidden="true">
  <div class="modal-dialog modal-xl modal-dialog-centered">
    <div class="modal-content">
      <div class="modal-header">
        <h5 class="modal-title" id="exampleModal3Label">Building a Graph of Cyber Knowledge </h5>
        <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Chiudi"></button>
      </div>
      <div class="modal-body">
The graph is constructed through a multi-layered pipeline that blends structure with semantics: 

Parsing MITRE ATT&CK data in STIX format (including techniques, malware, mitigations, groups, intrusion set). 

Named Entity Recognition (NER) to match abstract terms from 3,000+ research articles with MITRE concepts — generating “citation” edges. 

Topic modeling (LDA) to categorize disconnected articles into 10 macro cyber topics (e.g., Phishing & Machine Learning, Blockchain Security). 

Semantic similarity mapping using Sentence Transformers, linking articles to MITRE entities even when terms differ — capturing latent relations. 

Thematic clustering by connecting articles within the same topic. 

Export and visualization with Pyvis and Streamlit, including LLM-powered search via Mistral 7B. 
      </div>
      <div class="modal-footer">
        <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Chiudi</button>
      </div>
    </div>
  </div>
</div>


<div class="text-center my-3">
  <a href="javascript:void(0)"
     data-bs-toggle="modal"
     data-bs-target="#exampleModal4"
     class="modal-link">
    🛠 <span class="modal_link">Graph Metrics That Matter</span>
  </a>
</div>

<div class="modal fade" id="exampleModal4" tabindex="-1" aria-labelledby="exampleModal4Label" aria-hidden="true">
  <div class="modal-dialog modal-xl modal-dialog-centered">
    <div class="modal-content">
      <div class="modal-header">
        <h5 class="modal-title" id="exampleModal4Label"> Graph Metrics That Matter</h5>
        <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Chiudi"></button>
      </div>
      <div class="modal-body">
        The current version of the graph presents a robust, semantically rich topology: 
4,366 nodes, 296,187 edges confirming a dense and diverse relational space. 
Average path length: 3.77  concepts are quickly reachable from one another. 
Average clustering coefficient 0.5  strong local groupings of related content. 
PageRank peaks at 0.013 some articles act as high-authority knowledge hubs. 
Assortativity: +0.076 similar-degree nodes tend to connect, suggesting self-organized thematic coherence. 
These metrics confirm a navigable and highly interconnected ecosystem ideal for applications like RAG (Retrieval Augmented Generation), automated explanations, or exploratory training. 
      </div>
      <div class="modal-footer">
        <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Chiudi</button>
      </div>
    </div>
  </div>
</div>


###  From Attacks to Awareness: A Graph That Connects the Dots 
What begins as a cyberattack often ends in headlines, yet rarely in real understanding. Public narratives tend to dramatize, while companies react with urgency, investing in solutions they may not fully grasp. Somewhere between the breach and the boardroom, technical knowledge gets lost in translation. 

This is where our graph steps in: not just as a visualization tool, but as a way to connect data, expertise, and communication into a cohesive system of shared understanding. 
It links threats to research, concepts to countermeasures, and people to meaning, helping turn reactive defenses into informed strategies. 

Because in cybersecurity, visibility isn’t just about network logs — it’s about making knowledge itself visible. 

So the real question becomes: 
**Are we truly prepared? In the invisible war, who protects whom?**


# Conclusions {#conclusions}

## Research vs. Reality: Italy’s Cybersecurity Investments Under the Microscope  

Over the last decade, Italy has steadily climbed the European cybersecurity ladder, at least on paper. According to data from Horizon 2020 and Horizon Europe, the country ranks third in terms of net cybersecurity funding received, behind only Spain and Germany. From 2015 onward, Italy’s involvement in EU-backed research projects has grown consistently, peaking in 2021 with **115 active initiatives.**  

This trajectory suggests a country that, even before the surge in cyberattacks, was aware of the need to strengthen its digital defenses: a sign of strategic foresight in the face of accelerating digitalization.  

But while the research ecosystem expanded, so did the threats. **In 2023, Italy recorded its highest-ever number of cyberattacks against companies,** continuing a trend that began around 2021, the same period during which funding reached its peak.  

This overlap raises a critical and still unresolved question:  

### Are these investments paying off in the real world?  

At present, the answer is unclear. It’s possible the benefits of funding are simply delayed, that is that training, infrastructure, and innovation need time to convert into effective defense mechanisms. But another possibility looms: that **the translation of research into operational security is too slow, too fragmented, or even misaligned** with the actual needs of Italian businesses.  

This isn’t just a budgeting issue, it’s a structural one. The numbers tell one story, but they also invite a deeper investigation:  

### Does Italy’s cybersecurity model need a rethink? And if so, where should we start?  

To explore this further, we asked an **experienced voice in the cybersecurity field**  for their honest view on the situation. Here's what they shared:  

>As far as I know, the increase in projects hasn’t brought any significant or visible benefits. It mainly reflects better organizational capacity in the Italian ecosystem to apply for and manage funds. I haven’t seen more strategic selection of projects, nor clear impact in terms of cybersecurity outcomes or the emergence of new actors in the field.  
>For example, Spain has focused its funding on building infrastructure and labs. In contrast, in Italy, a large portion of funds has gone toward increasing precarious or part-time roles in public and private organizations. In the short term, this boosts fund usage rates, but in the long term, it brings little benefit — and even creates social costs, as we’re seeing in the academic sector.

Their words offer an honest reflection and leave us with a crucial, open-ended question:  

Will these investments eventually strengthen Italy’s cybersecurity landscape, or do we need to rethink how research is connected to real-world needs and resilience?” 


### A System That Knows — But Can It Act? 

This disconnect highlights a deeper issue: cybersecurity isn’t just a technical problem. It’s a systems problem spanning infrastructure, education, policy, communication, labor, and equity. 

We can’t protect what we don’t understand, and we can’t defend with isolated tools. 
**What we need is an ecological vision of cybersecurity**: one that connects institutions, individuals, technologies, and knowledge in a way that is resilient, transparent, and inclusive. 

Because the question is no longer whether the threats are real. 
It’s whether our response is coherent — and whether it reaches those who need it most. 

**TODO**: come ordinare questi grafici sotto?

<div style="display: flex; justify-content: center;">
  <div>
    <vegachart
      schema-url="{{ "/assets/charts/conclusions/ita_eu_average_fino_23_arancio.json" | relative_url }}"
      style="width: 100%; height: 100%"
      tooltip="true" >
    </vegachart>
  </div>
</div>

<div style="display: flex; justify-content: center;">
  <div>
    <vegachart
      schema-url="{{ "/assets/charts/conclusions/financig/chart_italy_projects.json" | relative_url }}"
      style="width: 100%; height: 100%"
      tooltip="true" >
    </vegachart>
  </div>
</div>

<div style="display: flex; justify-content: center;">
  <div>
    <vegachart
      schema-url="{{ "/assets/charts/conclusions/financig/chart_top10.json" | relative_url }}"
      style="width: 100%; height: 100%"
      tooltip="true" >
    </vegachart>
  </div>
</div>

<div style="display: flex; justify-content: center;">
  <div>
    <vegachart
      schema-url="{{ "/assets/charts/conclusions/financig/combined_chart.json" | relative_url }}"
      style="width: 100%; height: 100%"
      tooltip="true" >
    </vegachart>
  </div>
</div>

# About Us  {#about-us}

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incidunt ut labore et dolore magna aliqua.


<script>
document.querySelectorAll('.hm-btn1').forEach(btn=>{
  btn.addEventListener('click', ()=>{
    const target = btn.dataset.target;

    document.querySelectorAll('.hm-btn1').forEach(b=>b.classList.remove('active'));
    btn.classList.add('active');

    document.querySelectorAll('.heatmap').forEach(div=>div.classList.remove('visible'));
    document.getElementById(target).classList.add('visible');
  });
});
</script>


<script>
document.querySelectorAll('.hm-btn2').forEach(btn=>{
  btn.addEventListener('click', ()=>{
    const target = btn.dataset.target;

    document.querySelectorAll('.hm-btn2').forEach(b=>b.classList.remove('active'));
    btn.classList.add('active');

    document.querySelectorAll('.barchart').forEach(div=>div.classList.remove('visible'));
    document.getElementById(target).classList.add('visible');
  });
});
</script>