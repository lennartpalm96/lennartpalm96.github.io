---
title: 
layout: single
classes: wide
permalink: /side-projects/
---
<br/> 

<!-- Google Tag Manager (noscript) -->
<noscript><iframe src="https://www.googletagmanager.com/ns.html?id=GTM-PNS829G"
height="0" width="0" style="display:none;visibility:hidden"></iframe></noscript>
<!-- End Google Tag Manager (noscript) -->

# <center> Side Projects </center>
- - -

<div style="text-align: justify"><small>
Projects on topics I find interesting. These are AI-assisted explorations, built with Claude, that serve as starting points for future research ideas.
</small></div>
<br/>

**AI Adoption as a New Frontier of Regional Inequality in Korea**. 2026. Short paper <br><br/>
<small>[ <a href="#/" onclick="visib('ai-korea')">Abstract</a>] | [Paper][Palm_AI_Korea]] | [Replication package][Palm_AI_Korea_rep]] </small><br/>
<small><i>Built with AI: the analysis code, figures and text were developed with Claude.</i></small>

<div id="ai-korea" style="display: none; text-align: justify; line-height: 1.2" ><small>
 Generative AI use in Korea is far more concentrated in the Seoul Metropolitan Area (SMA) than population, output or wages. Combining the Anthropic Economic Index (Claude.ai, April–May 2026) with the Regional Employment Survey (second half of 2025), this paper shows that the SMA accounts for 83% of Korean Claude usage but only 51% of employment. Work use per worker is 1.68 times the national rate in the SMA and 0.24–0.39 in the three other macro regions.
 Occupational composition explains less than half of this gap. Within the same occupations, SMA usage is 2.4–3.1 times that of other regions, an order of magnitude more than the within-occupation gaps in wages or university degree shares (3–6%). The gap is as large among students, so it is likely to carry into the next cohort of workers. The exception is software, IT and data tasks, where usage is proportional to the relevant workforce in every region. This points to broader diffusion, rather than location as such, as the main policy lever.
 <br><br/>
 The replication package contains all code and data except the Regional Employment Survey microdata, which can be obtained from <a href="https://mdis.kostat.go.kr">MDIS</a> (Statistics Korea).
</small><br><br/>
</div>

[Palm_AI_Korea]: {{ site.baseurl }}{% link assets/files/Palm_AI_Regional_Inequality_Korea.pdf %}
[Palm_AI_Korea_rep]: {{ site.baseurl }}{% link assets/files/Palm_AI_Regional_Inequality_Korea_replication.zip %}

[//]: This java script is the button to show abstract
<script>
  function visib(id) {
     var x = document.getElementById(id);
     if (x.style.display === "block") {
          x.style.display = "none";
     } else {
          x.style.display = "block";
     }
  }
</script>
