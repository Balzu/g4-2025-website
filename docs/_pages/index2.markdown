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





# Map the Attack {#map-the-attack}


<div style="width: 800px; height: 500px;">
  <vegachart
    schema-url="{{ "/assets/charts/map_the_attack/attori_europa_black.json | relative_url }}"
    style="width: 100%; height: 100%" 
    tooltip="true" >
  </vegachart>
</div>



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