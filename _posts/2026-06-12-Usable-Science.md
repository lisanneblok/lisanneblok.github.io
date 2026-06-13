---
layout: post
title: "Usable science"
date: 2026-06-13
thumbnail: /images/chapman.png
keywords: [usability, conference]
excerpt: "Reflections on a conference for usable sea level projections"
---

<style>
  .post-hero { margin-bottom: 2rem; }

  .post-thumb-wrap {
    float: right;
    margin: 0 0 1.2rem 1.8rem;
    width: 340px;
    max-width: 50%;
  }

  .post-thumb-wrap img {
    width: 100%;
    border-radius: 10px;
    display: block;
    box-shadow: 0 4px 16px rgba(27,107,138,0.13);
  }

  .post-thumb-wrap figcaption {
    font-size: 0.75rem;
    color: #4a6070;
    text-align: center;
    margin-top: 0.4rem;
    font-style: italic;
  }

  .keyword-row {
    display: flex;
    flex-wrap: wrap;
    gap: 0.4rem;
    margin: 0 0 2rem;
  }

  .keyword-row span {
    font-size: 0.75rem;
    font-weight: 600;
    color: #1b6b8a;
    background: #e8f4f8;
    border: 1px solid #cfdde6;
    border-radius: 20px;
    padding: 0.2rem 0.7rem;
    font-family: system-ui, sans-serif;
  }

  .post-callout {
    border-left: 3px solid #1b6b8a;
    background: #e8f4f8;
    border-radius: 0 8px 8px 0;
    padding: 0.9rem 1.2rem;
    margin: 1.5rem 0;
    font-style: italic;
    color: #1a2634;
  }

  .post-divider {
    border: none;
    border-top: 2px solid #e8f4f8;
    margin: 2rem 0;
  }

  @media (max-width: 600px) {
    .post-thumb-wrap {
      float: none;
      width: 100%;
      max-width: 100%;
      margin: 0 0 1.2rem;
    }
  }
</style>

<!-- Keywords -->
<div class="keyword-row">
  {% for kw in page.keywords %}
  <span>{{ kw }}</span>
  {% endfor %}
</div>

<!-- Thumbnail wrapping into text -->
<figure class="post-thumb-wrap">
  <img src="{{ page.thumbnail }}" alt="{{ page.title }}">
  <figcaption>Where science could/should end up</figcaption>
</figure>

## Usable science
Last week, I attended a conference on "usable" sea level projections. The conference was attended by a range of practitioners (translators of science to local communities and councils), scientists, and NGO's. It started off as a large conference with the authors of the International Panel of Climate Change report, but quickly raised questions on how this science could be presented. The scientists quickly understood that "low confidence, high likelihood", and a unlikely worst-case scenario, might also be confusing to us. The real questions arised: what complexity, and how much detail, should be included to inform policy-makers?

<div style="clear:both"></div>

<hr class="post-divider">

#### Complexity
Where usable science arguably is a clear outcome, predicting the future is very complex. First of all, it is very difficult to test and validate whether the models used are accurate. In the context of sea level, the modelling framework is an interplay of very small models, ranging from ice sheets, glaciers, and rivers, to the movement of water due to land vertical movement. This gives rise to a number of sources of uncertainty: from the lack of data and modelling quality, as well as a lack of knowledge. Climate and weather can also be a bit "random", thus the models need to be run multiple times to account for any dynamics that might be missed. Looking at the range of possible outcomes, from a large number of model runs is what we call an "ensemble". Usually, scientists take the average value of this ensemble, as this would be the most likely outcome, but take the variability of these outcomes into account to look at the confidence.

Another large uncertainty is **policy-based climate mitigation**, where the decisions made can impact the CO2 emissions, as well as socio-economic response to climate change. Therefore, climate scientists run a large number of simulations, under these future scenarios.

<!-- Callout / pull-quote block -->
<div class="post-callout">
  "How high is the sea going to be in 2100?" Do I need to build a 2 metre dyke? What future flood line do I use for insurance purposes?
</div>

Stay tuned for more reflections, including a recent trip to a "usable science" conference in Montreal!

<hr class="post-divider">

#### A red thread
On the practitioner panel, one thing became clear: those projections until 2300 are not relevant to communities and coastal populations NOW. Let alone can politicians use any projections when the research is so uncertain about future projections.

#### Summary for Policy-Makers
So from all this complex analysis in the IPCC, what should be communicated to policy-makers, and what complexity is helpful? And is this up to the scientists to decide?
