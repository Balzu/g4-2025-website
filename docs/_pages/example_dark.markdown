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
</style>


# Introduction

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incidunt ut labore et dolore magna aliqua.

# Map the Hack

![Infografica]({{ "/assets/images/infografica.png" | relative_url }})

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incidunt ut labore et dolore magna aliqua.

# Breaking the Net

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incidunt ut labore et dolore magna aliqua.

<div style="height: 400px">
  <vegachart
    schema-url="{{ "/assets/charts/articles_by_source_type.json" | relative_url }}"
    style="width: 100%; height: 100%">
  </vegachart>
</div>

<div style="height: 400px">
  <vegachart
    schema-url="{{ "/assets/charts/normalized_coverage_per_attack.json" | relative_url }}"
    style="width: 100%; height: 100%">
  </vegachart>
</div>



<div id="vis" style="height:400px;"></div>

<script>
  vegaEmbed(
    '#vis',
    '{{ "/assets/charts/italia.json" | relative_url }}',
    {
      renderer:  'canvas',   // o 'svg'
      tooltip:   true,       // abilita vega-tooltip
      actions: {
        export: true,        // bottone “Download as PNG/SVG”
        source: false        // nasconde il pulsante “View Source”
      }
    }
  ).catch(console.error);
</script>



# Cyber Q&A

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incidunt ut labore et dolore magna aliqua.

# Conclusions

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incidunt ut labore et dolore magna aliqua.

# About Us

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incidunt ut labore et dolore magna aliqua.
