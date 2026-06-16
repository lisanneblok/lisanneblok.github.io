---
layout: page
title: About Me
permalink: /resume/
---

<style>
  /* ── Tokens ── */
  :root {
    --ink:       #1a2634;
    --muted:     #4a6070;
    --accent:    #1b6b8a;
    --accent-lt: #e8f4f8;
    --border:    #cfdde6;
    --bg:        #f7fbfd;
    --card-bg:   #ffffff;
    --radius:    10px;
    --font-body: 'Georgia', serif;
    --font-ui:   system-ui, -apple-system, sans-serif;
  }

  /* ── Reset ── */
  .cv-wrap * { box-sizing: border-box; margin: 0; padding: 0; }

  /* ── Outer layout ── */
  .cv-wrap {
    font-family: var(--font-body);
    color: var(--ink);
    background: var(--bg);
    max-width: 960px;
    margin: 2rem auto;
    padding: 0 1rem;
  }

  /* ── Hero: photo wraps left, text flows right ── */
  .hero {
    margin-bottom: 2.5rem;
    overflow: hidden; /* clearfix for float */
  }

  .profile-pic {
    float: left;
    width: 180px;
    height: 180px;
    object-fit: cover;
    border-radius: 50%;
    border: 3px solid var(--accent);
    margin: 0 1.8rem 1rem 0;
    shape-outside: circle(50%);
  }

  .hero h1 {
    font-family: var(--font-ui);
    font-size: 2rem;
    font-weight: 700;
    color: var(--ink);
    line-height: 1.2;
    margin-bottom: 0.25rem;
  }

  .hero .subtitle {
    font-family: var(--font-ui);
    font-size: 0.95rem;
    color: var(--accent);
    letter-spacing: 0.04em;
    font-weight: 600;
    margin-bottom: 0.8rem;
    text-transform: uppercase;
  }

  .hero p {
    font-size: 1rem;
    line-height: 1.7;
    color: var(--muted);
    margin-bottom: 0.75rem;
  }

  /* ── Contact pill row ── */
  .contact-row {
    display: flex;
    flex-wrap: wrap;
    gap: 0.5rem;
    margin-top: 0.75rem;
    clear: none;
  }

  .contact-row a {
    display: inline-block;
    font-family: var(--font-ui);
    font-size: 0.8rem;
    font-weight: 600;
    color: var(--accent);
    background: var(--accent-lt);
    border: 1px solid var(--border);
    border-radius: 20px;
    padding: 0.25rem 0.85rem;
    text-decoration: none;
    transition: background 0.15s, color 0.15s;
  }

  .contact-row a:hover {
    background: var(--accent);
    color: #fff;
    border-color: var(--accent);
  }

  /* ── Section heading ── */
  .section-label {
    font-family: var(--font-ui);
    font-size: 0.72rem;
    font-weight: 700;
    letter-spacing: 0.12em;
    text-transform: uppercase;
    color: var(--accent);
    margin-bottom: 0.85rem;
    padding-bottom: 0.4rem;
    border-bottom: 2px solid var(--accent-lt);
  }

  /* ── Card grid ── */
   .card-grid {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 1rem;
    margin-bottom: 2rem;
  }

  .card {
    background: var(--card-bg);
    border: 1px solid var(--border);
    border-radius: var(--radius);
    padding: 1.1rem 1.2rem;
    box-shadow: 0 2px 6px rgba(27,107,138,0.06);
    transition: box-shadow 0.2s, transform 0.2s;
  }

  .card:hover {
    box-shadow: 0 5px 18px rgba(27,107,138,0.13);
    transform: translateY(-2px);
  }

  .card h3 {
    font-family: var(--font-ui);
    font-size: 0.8rem;
    font-weight: 700;
    letter-spacing: 0.08em;
    text-transform: uppercase;
    color: var(--accent);
    margin-bottom: 0.65rem;
  }

  .card ul {
    list-style: none;
    padding: 0;
  }

  .card ul li {
    font-family: var(--font-ui);
    font-size: 0.875rem;
    color: var(--ink);
    padding: 0.22rem 0;
    border-bottom: 1px solid var(--accent-lt);
    line-height: 1.4;
  }

  .card ul li:last-child { border-bottom: none; }

  /* ── Skills card (tag cloud style) ── */
  .skills-card {
    background: var(--card-bg);
    border: 1px solid var(--border);
    border-radius: var(--radius);
    padding: 1.1rem 1.2rem;
    margin-bottom: 2rem;
    box-shadow: 0 2px 6px rgba(27,107,138,0.06);
  }

  .skills-card h3 {
    font-family: var(--font-ui);
    font-size: 0.8rem;
    font-weight: 700;
    letter-spacing: 0.08em;
    text-transform: uppercase;
    color: var(--accent);
    margin-bottom: 0.75rem;
  }

  .tag-row {
    display: flex;
    flex-wrap: wrap;
    gap: 0.45rem;
  }

  .tag {
    font-family: var(--font-ui);
    font-size: 0.8rem;
    font-weight: 600;
    color: var(--accent);
    background: var(--accent-lt);
    border: 1px solid var(--border);
    border-radius: 6px;
    padding: 0.25rem 0.7rem;
  }

  /* ── Publications & Outside Research ── */
  .prose-section {
    background: var(--card-bg);
    border: 1px solid var(--border);
    border-radius: var(--radius);
    padding: 1.3rem 1.4rem;
    margin-bottom: 1.2rem;
    box-shadow: 0 2px 6px rgba(27,107,138,0.06);
  }

  .prose-section p {
    font-size: 0.95rem;
    line-height: 1.7;
    color: var(--muted);
  }

  .prose-section a {
    color: var(--accent);
    font-weight: 600;
    text-decoration: none;
  }

  .prose-section a:hover { text-decoration: underline; }

  /* ── Responsive ── */
  @media (max-width: 600px) {
    .profile-pic {
      float: none;
      display: block;
      margin: 0 auto 1.2rem;
    }
    .hero h1 { font-size: 1.5rem; }
    .card-grid { grid-template-columns: 1fr; }
  }
</style>

<div class="cv-wrap">

  <!-- ── Hero ── -->
  <div class="hero">
    <img src="/images/introplot.png" alt="Lisanne Blok" class="profile-pic">
    <h1>Lisanne Blok</h1>
    <p class="subtitle">PhD Student · AI for Environmental Risk · University of Cambridge</p>
    <p>
      I am a PhD student researching extreme sea level and coastal flooding.
      My work focuses on generating evidence that can support policy-making
      and improve resilience to environmental hazards.
    </p>
    <p>
      I am particularly interested in the science–policy interface:
      how scientists can generate policy-relevant evidence, how evidence is incorporated
      into decision-making, and how scientific findings can be communicated effectively.
    </p>
    <div class="contact-row">
      <a href="mailto:lb962@cam.ac.uk">✉ Email</a>
      <a href="https://orcid.org/0009-0006-5944-4169">ORCID</a>
      <a href="https://github.com/lisanneblok">GitHub</a>
      <a href="https://linkedin.com">LinkedIn</a>
    </div>
  </div>

  <!-- ── Skills ── -->
  <p class="section-label">Skills</p>
  <div class="skills-card">
    <div class="tag-row">
      <span class="tag">Python</span>
      <span class="tag">R</span>
      <span class="tag">Excel</span>
      <span class="tag">Machine Learning</span>
      <span class="tag">Data Analysis</span>
      <span class="tag">Policy Analysis</span>
      <span class="tag">Public Speaking</span>
      <span class="tag">Scientific Communication</span>
    </div>
  </div>

  <!-- ── Info cards ── -->
  <p class="section-label">Overview</p>
  <div class="card-grid">

    <div class="card">
      <h3>Experience</h3>
      <ul>
        <li>PhD Intern — Defra UK Government (2026)</li>
        <li>Bangladesh Heatwaves — Imperial College London</li>
        <li>Social Cost of Carbon — Grantham Institute</li>
        <li>Summer Placement — Institute of Economic Affairs</li>
      </ul>
    </div>

    <div class="card">
      <h3>Education</h3>
      <ul>
        <li>PhD AI for Environmental Risk — Cambridge</li>
        <li>MRes Environmental Data Science — Cambridge</li>
        <li>BSc Geophysics — Imperial College London</li>
        <li>English, German, and French language certificates</li>
      </ul>
    </div>

    <div class="card">
      <h3>Research Interests</h3>
      <ul>
        <li>Extreme Sea Levels</li>
        <li>Coastal Flooding</li>
        <li>Environmental Risk</li>
        <li>Science Policy</li>
        <li>Climate Adaptation</li>
        <li>Environmental AI</li>
      </ul>
    </div>

    <div class="card">
      <h3>Current Projects</h3>
      <ul>
        <li>Marine Litter &amp; Policy Implications</li>
        <li>Drivers of Surge Regimes</li>
        <li>Extreme Sea Level Variability</li>
        <li>Earthquake Impact Assessment in Myanmar</li>
      </ul>
    </div>

  </div>

  <!-- ── Publications ── -->
  <p class="section-label">Publications &amp; Research Outputs</p>
  <div class="prose-section">
    <p>
      View my full list of publications and outputs on my
      <a href="https://orcid.org/0009-0006-5944-4169">ORCID profile</a>.
    </p>
  </div>

  <!-- ── Outside Research ── -->
  <p class="section-label">Outside Research</p>
  <div class="prose-section">
    <p>I enjoy sailing, rowing, and spending time on the water.</p>
  </div>

</div>
