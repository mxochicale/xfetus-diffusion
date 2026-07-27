Miguel Xochicale

# 

<div style="background-color: rgba(22,22,22,0.75);   border-radius: 10px;   text-align:center;   padding: 0px;   padding-left: 1.5em;   padding-right: 1.5em;   max-width: max-content;   margin-left: auto;   margin-right: auto;   padding-top: 0.2em;   padding-bottom: 0.2em;   line-height: 1.5em!important;">

<span style="color:#939393; font-size:1.75em; text-align:left; display:block;">

<!-- TODO: replace with the real talk title -->

<span style="color:#e0e0e0; font-size:1.65em; display:block; font-weight:600;">Foundation
Diffusion Model with Open-Source Medical Imaging in Unified-AI</span>

</span>

------------------------------------------------------------------------

<span style="font-size:0.55em; color:#aaaaaa;">[**Miguel Xochicale (
@mxochicale)** ](https://github.com/mxochicale), Senior RSE,
[UCL-ARC](https://www.ucl.ac.uk/advanced-research-computing/)</span>

</div>

<div class="footer">

<span class="dim-text" style="text-align:left;">Q1-2026 [(web-animations
2025 by
mxochicale)](https://mxochicale.github.io/web-animations/)</span>

</div>

<div class="notes">

<!-- TODO: add opening speaker notes -->

</div>

<!-- ============================================================
     OVERVIEW
     ============================================================ -->

## Overview

<div class="columns">

<div class="column" width="50%">

<!-- TODO: link items 3-4 to real slide anchors once those sections exist,
     e.g. add `{#sectag_demos}` / `{#sectag_future}` to their section headers -->

- [My journey](#secMJ)
- [Prenatal ultrasound (US) Imaging](#secUS) <add details>
- [EDM2 diffusion model](#secDM) <add details>
- [Image Quality Assessment](#secIQ) <add details>
- [Unified-AI](#secUAI) <add details>
- [Future Work](#secFW) <add details>

</div>

<div class="column" width="50%">

</div>

</div>

<div class="notes">

<!-- TODO: add key themes -->

### What We’ll Cover

### Key Themes

<!-- TODO: replace placeholder keywords -->

> [!NOTE]
>
> ### :cloud: Cloud keywords
>
> keyword1, keyword2, keyword3

> [!TIP]
>
> ### :robot: Robotics keywords
>
> keyword1, keyword2, keyword3

> [!IMPORTANT]
>
> ### :busts_in_silhouette: Collaborative keywords
>
> keyword1, keyword2, keyword3

</div>

<!-- *********************** NEW SLIDE *********************** -->

## My Journey

<img src="figures/mx.png" style="width:100.0%"
data-fig-align="center" />

<div class="notes">

To update figure go to:
https://github.com/mxochicale/cv/tree/main/my-journey

</div>

<!-- ============================================================
     SECTION: Section 1
     ============================================================ -->

# Prenatal ultrasound (US) Imaging

**Add Subtitle**

<div class="notes">

<!-- TODO: notes specific to Section title 1 -->

Walk through the three layers: cloud VMs managed via Terraform/k8s, the
campus network, and physical hardware (sensors, robots).

</div>

<!-- *********************** NEW SLIDE *********************** -->

##  Github: Getting started docs

<div id="fig-template-section1">

<img src="figures/00_template-vector-images/drawing-v00.svg"
data-fig-align="center" />

Figure 1: Getting started documentation provide with a range of links to
setup, use, run and debug application including github workflow.

</div>

<div class="notes">

Speaker notes go here.

</div>

<!-- ============================================================
     SECTION: Section 2
     ============================================================ -->

# EDM2 diffusion model

Elucidating the Design Space of Diffusion Models, version 2\
Harvey Mannering

<div class="notes">

<!-- TODO: notes specific to Section title 1 -->

Gigaflops per evaluation measures computational efficiency by tracking
how many billions of floating-point math calculations (gigaflops) a
computer processor uses to test, score, or run a single trial
(evaluation) in an algorithm or model.

</div>

<!-- *********************** NEW SLIDE *********************** -->

## What Are Diffusion Models?

<div id="fig-template-section1">

<img src="figures/diffusion_models.svg" data-fig-align="center" />

Figure 2: Overview of different types of generative models. (Source:
[Lil’Log](https://lilianweng.github.io/posts/2021-07-11-diffusion-models/))

</div>

<div class="notes">

Speaker notes go here.

https://lilianweng.github.io/posts/2021-07-11-diffusion-models/
https://toloka.ai/blog/unveiling-the-dynamics/

</div>

<!-- *********************** NEW SLIDE *********************** -->

## EDM2: Record quality at fraction of training time

<div id="fig-template-section1">

<img src="figures/edm2_fig1.svg" data-fig-align="center" />

Figure 3: Figure 1 from Kerras et al. 2024 in CVPR.

</div>

<div class="notes">

Speaker notes go here.

PAPER: https://arxiv.org/pdf/2312.02696 POSTER:
https://cvpr.thecvf.com/virtual/2024/poster/31235

</div>

<!-- *********************** NEW SLIDE *********************** -->

## EDM2 Architecture

<div id="fig-template-section1">

<img src="figures/edm2_fig2.svg" data-fig-align="center" />

Figure 4: Figure 2 EDM2 Architecture combines a U-Net with
self-attention layers (Kerras et al. 2024 in CVPR).

</div>

<div class="notes">

Speaker notes go here.

PAPER: https://arxiv.org/pdf/2312.02696 POSTER:
https://cvpr.thecvf.com/virtual/2024/poster/31235

</div>

<!-- *********************** NEW SLIDE *********************** -->

## EDM2 Results

<div id="fig-template-section1">

<img src="figures/edm2_table2.svg" data-fig-align="center" />

Figure 5: Table 2. Results on ImageNet-512. “EDM2-S” is the same as
CONFIG G in Table 1 (Kerras et al. 2024 in CVPR).

</div>

<div class="notes">

Speaker notes go here.

PAPER: https://arxiv.org/pdf/2312.02696 POSTER:
https://cvpr.thecvf.com/virtual/2024/poster/31235

TODO

- OUR PAPER We train two different sized networks, EDM2-S and EDM2-XL,
  which allows us to apply autoguidance \[14\] to improve image quality.

- KERAS2024: In our tests, the smallest (XS) unconditional model was
  found to be sufficient for guiding even the largest (XXL) conditional
  model — using a larger unconditional model did not improve the results
  at all.

</div>

<!-- ============================================================
     SECTION: Section 3
     ============================================================ -->

# Image Quality Assessment

**Add Subtitle**

<div class="notes">

<!-- TODO: notes specific to Section title 1 -->

Walk through the three layers: cloud VMs managed via Terraform/k8s, the
campus network, and physical hardware (sensors, robots).

</div>

<!-- *********************** NEW SLIDE *********************** -->

##  Github: Getting started docs

<div id="fig-template-section1">

<img src="figures/00_template-vector-images/drawing-v00.svg"
data-fig-align="center" />

Figure 6: Getting started documentation provide with a range of links to
setup, use, run and debug application including github workflow.

</div>

<div class="notes">

Speaker notes go here.

</div>

<!-- ============================================================
     SECTION: Section 4
     ============================================================ -->

# Unified-AI

**Add Subtitle**

<div class="notes">

<!-- TODO: notes specific to Section title 1 -->

Walk through the three layers: cloud VMs managed via Terraform/k8s, the
campus network, and physical hardware (sensors, robots).

</div>

<!-- *********************** NEW SLIDE *********************** -->

##  Github: Getting started docs

<div id="fig-template-section1">

<img src="figures/00_template-vector-images/drawing-v00.svg"
data-fig-align="center" />

Figure 7: Getting started documentation provide with a range of links to
setup, use, run and debug application including github workflow.

</div>

<div class="notes">

Speaker notes go here.

</div>

<!-- ============================================================
     SECTION: Section 5
     ============================================================ -->

# Future Work

**Add Subtitle**

<div class="notes">

<!-- TODO: notes specific to Section title 2 (was previously a duplicate
     of Section title 1's notes — make sure this describes section 2) -->

</div>

<!-- *********************** NEW SLIDE *********************** -->

##  Github: Getting started docs

<div id="fig-template-section2">

<img src="figures/00_template-vector-images/drawing-v00.svg"
data-fig-align="center" />

Figure 8: Getting started documentation provide with a range of links to
setup, use, run and debug application including github workflow.

</div>

<div class="notes">

Speaker notes go here.

</div>

<!-- *********************** NEW SLIDE *********************** -->

## Title of the slide

- Bullet point 1
- Bullet point 2
- **Bullet point** 3
  - Bullet point 3.1
  - Bullet point 3.2

<div style="font-size: 55%;">

**Sciortino et al. 2017** in Computers in Biology and Medicine
<https://doi.org/10.1016/j.compbiomed.2017.01.008> **He et al. 2021** in
Front. Med. <https://doi.org/10.3389/fmed.2021.729978>

</div>

<div class="notes">

Notes go here

</div>

<!-- ============================================================
     EXTRA SLIDES (appendix)
     ============================================================ -->

# Appendix

Extra slides for Q&A

<!-- *********************** NEW SLIDE *********************** -->

## Title of the slide

- Bullet point 1
- Bullet point 2
- **Bullet point** 3
  - Bullet point 3.1
  - Bullet point 3.2

<div style="font-size: 55%;">

**Sciortino et al. 2017** in Computers in Biology and Medicine
<https://doi.org/10.1016/j.compbiomed.2017.01.008> **He et al. 2021** in
Front. Med. <https://doi.org/10.3389/fmed.2021.729978>

</div>

<div class="notes">

Notes go here

</div>
