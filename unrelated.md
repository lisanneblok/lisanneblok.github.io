---
layout: page

permalink: /unrelated/
---

<link href="/css/override.css" rel="stylesheet" type="text/css">
<style>
  :root {
    --ink:       #1a2634;
    --muted:     #4a6070;
    --accent:    #1b6b8a;
    --accent-lt: #e8f4f8;
    --border:    #cfdde6;
    --card-bg:   #ffffff;
    --radius:    10px;
    --font-body: 'Georgia', serif;
    --font-ui:   system-ui, -apple-system, sans-serif;
  }

  .ut-wrap {
    max-width: 720px;
    margin: 2rem auto;
    padding: 0 1rem;
    font-family: var(--font-body);
    color: var(--ink);
  }

  /* ── Hero ── */
  .ut-hero {
    margin-bottom: 2.5rem;
    border-bottom: 2px solid var(--accent-lt);
    padding-bottom: 1.5rem;
  }
  .ut-hero__eyebrow {
    font-family: var(--font-ui);
    font-size: 0.72rem;
    font-weight: 700;
    letter-spacing: 0.14em;
    text-transform: uppercase;
    color: var(--accent);
    margin-bottom: 0.6rem;
  }
  .ut-hero__title {
    font-family: var(--font-ui);
    font-size: 2rem;
    font-weight: 800;
    color: var(--ink);
    margin: 0 0 0.75rem;
    line-height: 1.15;
  }
  .ut-hero__sub {
    font-size: 1.05rem;
    color: var(--muted);
    line-height: 1.7;
    max-width: 560px;
    margin: 0;
  }

  /* ── Section headers ── */
  .ut-section {
    margin-bottom: 2.2rem;
  }
  .ut-section__label {
    font-family: var(--font-ui);
    font-size: 0.7rem;
    font-weight: 700;
    letter-spacing: 0.13em;
    text-transform: uppercase;
    color: var(--accent);
    border-bottom: 2px solid var(--accent-lt);
    padding-bottom: 0.35rem;
    margin-bottom: 1rem;
  }

  /* ── Prose ── */
  .ut-prose {
    font-size: 0.97rem;
    line-height: 1.75;
    color: var(--muted);
  }
  .ut-prose p { margin: 0 0 1rem; }
  .ut-prose p:last-child { margin-bottom: 0; }

  /* ── Pill tags ── */
  .ut-tags {
    display: flex;
    flex-wrap: wrap;
    gap: 0.5rem;
    margin-top: 0.75rem;
  }
  .ut-tag {
    font-family: var(--font-ui);
    font-size: 0.78rem;
    font-weight: 600;
    background: var(--accent-lt);
    color: var(--accent);
    border: 1px solid var(--border);
    border-radius: 20px;
    padding: 0.25rem 0.8rem;
  }

  /* ── List cards ── */
  .ut-list {
    list-style: none;
    margin: 0;
    padding: 0;
    display: flex;
    flex-direction: column;
    gap: 0.65rem;
  }
  .ut-list li {
    background: var(--card-bg);
    border: 1px solid var(--border);
    border-radius: var(--radius);
    padding: 0.75rem 1rem;
    font-size: 0.93rem;
    color: var(--muted);
    line-height: 1.5;
    box-shadow: 0 1px 4px rgba(27,107,138,0.05);
  }
  .ut-list li strong {
    color: var(--ink);
    font-family: var(--font-ui);
    font-size: 0.82rem;
    font-weight: 700;
    display: block;
    margin-bottom: 0.2rem;
  }

  /* ── Currently card ── */
  .ut-currently {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 0.75rem;
  }
  @media (max-width: 600px) {
    .ut-currently { grid-template-columns: 1fr; }
  }
  .ut-now-card {
    background: var(--card-bg);
    border: 1px solid var(--border);
    border-radius: var(--radius);
    padding: 0.9rem 1rem;
    box-shadow: 0 1px 4px rgba(27,107,138,0.05);
  }
  .ut-now-card__icon {
    font-size: 1.3rem;
    margin-bottom: 0.35rem;
  }
  .ut-now-card__label {
    font-family: var(--font-ui);
    font-size: 0.65rem;
    font-weight: 700;
    letter-spacing: 0.1em;
    text-transform: uppercase;
    color: var(--accent);
    margin-bottom: 0.2rem;
  }
  .ut-now-card__value {
    font-family: var(--font-body);
    font-size: 0.92rem;
    color: var(--ink);
    line-height: 1.4;
  }
</style>

<div class="ut-wrap">

  <!-- Hero -->
  <div class="ut-hero">
    <p class="ut-hero__eyebrow">Beyond the lab</p>
    <h1 class="ut-hero__title">Unrelated Thoughts</h1>
    <p class="ut-hero__sub">
      Not everything worth saying is about science or policy. 
      Here's the rest of it — hobbies, books, half-formed opinions, 
      and whatever else is on my mind (feminism, politics, sports).
    </p>
  </div>

  <!-- Currently into -->
  <div class="ut-section">
    <p class="ut-section__label">Currently</p>
    <div class="ut-currently">
      <div class="ut-now-card">
        <div class="ut-now-card__icon">📖</div>
        <p class="ut-now-card__label">Reading</p>
        <p class="ut-now-card__value">"Goddesses in Greek Myth"</p>
      </div>
      <div class="ut-now-card">
        <div class="ut-now-card__icon">🎵</div>
        <p class="ut-now-card__label">Listening to</p>
        <p class="ut-now-card__value">Alex Warren, and my own songs!</p>
      </div>
      <div class="ut-now-card">
        <div class="ut-now-card__icon">🌍</div>
        <p class="ut-now-card__label">Last travelled to</p>
        <p class="ut-now-card__value">Dublin, and Montréal</p>
      </div>
      <div class="ut-now-card">
        <div class="ut-now-card__icon">🧪</div>
        <p class="ut-now-card__label">Cooking / making</p>
        <p class="ut-now-card__value">Follow me: https://www.instagram.com/lisannecambridge/)</p>
      </div>
    </div>
  </div>

  <!-- Hobbies -->
  <div class="ut-section">
    <p class="ut-section__label">Things I do for fun</p>
    <div class="ut-prose">
      <p>Even though my PhD and work are water-related, I also like to spend my free time there!</p>
    </div>
    <div class="ut-tags">
      <span class="ut-tag">🚣 Rowing</span>
      <span class="ut-tag">⛵ Sailing</span>
      <span class="ut-tag">🍳 Cooking</span>
      <span class="ut-tag">🎤🎸 Writing and playing music</span>
    </div>
  </div>

  <!-- Opinions / takes -->
  <div class="ut-section">
    <p class="ut-section__label">Mild opinions</p>
    <ul class="ut-list">
      <li>
        <strong>On something cultural</strong>
        What role should young men and women play for feminism, and what discussions are the first one to be had? And should politics and men "protect" women from objectification, or is that a choice the women can make themselves?
      </li>
      <li>
        <strong>On something everyday</strong>
        Should we be watching the FIFA world cup with its corruption and political implications, where fans aren't even let into the country?
      </li>
      <li>
        <strong>On something you've changed your mind about</strong>
        The fact that you don't always have to say yes to every opportunity, and that self-care and time alone can be as valuable as the dinner/conference/travel you'd be missing out on.
      </li>
    </ul>
  </div>

 <!-- Recommendations -->
  <div class="ut-section">
    <p class="ut-section__label">Things worth your time</p>
    <ul class="ut-list">
      <li>
        <strong>A book</strong>
        Yesteryear - Claro Clare Burke. Thoughts on trad wives?
      </li>
      <li>
        <strong>A film or series</strong>
        Salt, Fat, Acid, Heat on the most important considerations for making flavourful food!
      </li>
      <li>
        <strong>A recipe</strong>
        Creamy tomato orzo, as it mostly uses cupboard items and takes up 20 minutes of your time!
      </li>
      <li>
        <strong>Something online</strong>
        World in data, where statistics drive policy analysis (https://ourworldindata.org/)
      </li>
    </ul>
  </div>

</div>
