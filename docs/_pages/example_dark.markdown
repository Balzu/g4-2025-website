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

</style>


# Introduction

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incidunt ut labore et dolore magna aliqua.

# Map the Hack

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


# Breaking the Net

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incidunt ut labore et dolore magna aliqua.


<div>
  <vegachart
    schema-url="{{ "/assets/charts/articles_by_source_type.json" | relative_url }}"
    style="width: 100%; height: 100%" 
    tooltip="true" >
  </vegachart>
</div>




# Cyber Q&A

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incidunt ut labore et dolore magna aliqua.

# Conclusions

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incidunt ut labore et dolore magna aliqua.

# About Us

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