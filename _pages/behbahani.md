---
layout: page
title: Behbahani
permalink: /behbahani/
nav: true
nav_order: 5
---

<style>
  .behbahani-page {
    --card-border: rgba(128, 128, 128, 0.16);
    --soft-bg: rgba(128, 128, 128, 0.055);
    --softer-bg: rgba(128, 128, 128, 0.035);
    --accent-soft: color-mix(in srgb, var(--global-theme-color) 12%, transparent);
  }

  .behbahani-hero {
    position: relative;
    padding: 2.2rem 2rem;
    margin: 0.5rem 0 2.5rem 0;
    border: 1px solid var(--card-border);
    border-radius: 1.4rem;
    background:
      radial-gradient(circle at top right, var(--accent-soft), transparent 34%),
      linear-gradient(135deg, rgba(128, 128, 128, 0.07), rgba(128, 128, 128, 0.02));
    overflow: hidden;
  }

  .behbahani-hero::after {
    content: "";
    position: absolute;
    right: -3.5rem;
    bottom: -3.5rem;
    width: 12rem;
    height: 12rem;
    border-radius: 999px;
    border: 1px solid rgba(128, 128, 128, 0.12);
    background: rgba(128, 128, 128, 0.025);
  }

  .behbahani-kicker {
    display: inline-block;
    margin-bottom: 0.85rem;
    padding: 0.28rem 0.72rem;
    border-radius: 999px;
    font-size: 0.74rem;
    font-weight: 700;
    letter-spacing: 0.08em;
    text-transform: uppercase;
    color: var(--global-theme-color);
    background-color: rgba(128, 128, 128, 0.09);
    border: 1px solid rgba(128, 128, 128, 0.14);
  }

  .behbahani-hero h2 {
    margin: 0 0 0.85rem 0;
    font-size: clamp(1.65rem, 3vw, 2.35rem);
    line-height: 1.15;
    letter-spacing: -0.02em;
  }

  .behbahani-hero p {
    max-width: 760px;
    margin-bottom: 0;
    font-size: 1.02rem;
    line-height: 1.68;
    opacity: 0.88;
  }

  .behbahani-tags {
    display: flex;
    flex-wrap: wrap;
    gap: 0.45rem;
    margin-top: 1.35rem;
  }

  .behbahani-tag {
    display: inline-block;
    padding: 0.28rem 0.7rem;
    border-radius: 999px;
    font-size: 0.78rem;
    font-weight: 600;
    color: var(--global-text-color);
    background-color: var(--global-bg-color);
    border: 1px solid var(--card-border);
  }

  .behbahani-section {
    margin: 2.4rem 0;
  }

  .behbahani-section h2 {
    margin-bottom: 0.75rem;
  }

  .behbahani-section-intro {
    max-width: 780px;
    margin-bottom: 1.25rem;
    line-height: 1.65;
    opacity: 0.82;
  }

  .behbahani-grid {
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));
    gap: 1rem;
    margin-top: 1.25rem;
  }

  .behbahani-card {
    padding: 1.15rem 1.15rem 1.05rem 1.15rem;
    border: 1px solid var(--card-border);
    border-radius: 1rem;
    background-color: var(--softer-bg);
    transition: transform 160ms ease, background-color 160ms ease, border-color 160ms ease;
  }

  .behbahani-card:hover {
    transform: translateY(-2px);
    background-color: var(--soft-bg);
    border-color: rgba(128, 128, 128, 0.26);
  }

  .behbahani-card h3 {
    margin: 0 0 0.55rem 0;
    font-size: 0.98rem;
    color: var(--global-theme-color);
  }

  .behbahani-card p {
    margin: 0;
    font-size: 0.91rem;
    line-height: 1.55;
    opacity: 0.84;
  }

  .behbahani-highlight {
    padding: 1.35rem 1.45rem;
    margin: 1.75rem 0;
    border-left: 4px solid var(--global-theme-color);
    border-radius: 0.85rem;
    background-color: var(--soft-bg);
  }

  .behbahani-highlight p {
    margin: 0;
    line-height: 1.65;
    opacity: 0.88;
  }

  .behbahani-research-list {
    display: grid;
    grid-template-columns: 1fr;
    gap: 0.75rem;
    margin-top: 1.25rem;
  }

  .behbahani-research-item {
    display: grid;
    grid-template-columns: 11rem 1fr;
    gap: 1rem;
    padding: 1rem 1.1rem;
    border: 1px solid var(--card-border);
    border-radius: 0.95rem;
    background-color: rgba(128, 128, 128, 0.03);
  }

  .behbahani-research-item strong {
    color: var(--global-theme-color);
  }

  .behbahani-research-item span {
    line-height: 1.55;
    opacity: 0.84;
  }

  .behbahani-resource-wrap {
    display: grid;
    grid-template-columns: repeat(2, minmax(0, 1fr));
    gap: 1rem;
    margin-top: 1.25rem;
  }

  .behbahani-resource {
    padding: 1.2rem;
    border: 1px solid var(--card-border);
    border-radius: 1rem;
    background:
      linear-gradient(180deg, rgba(128, 128, 128, 0.055), rgba(128, 128, 128, 0.02));
  }

  .behbahani-resource h3 {
    margin-top: 0;
    margin-bottom: 0.5rem;
    font-size: 1rem;
  }

  .behbahani-resource p {
    margin-bottom: 0.85rem;
    font-size: 0.92rem;
    line-height: 1.58;
    opacity: 0.84;
  }

  .status-badge {
    display: inline-block;
    padding: 0.25rem 0.62rem;
    border-radius: 999px;
    font-size: 0.72rem;
    font-weight: 700;
    letter-spacing: 0.04em;
    text-transform: uppercase;
    color: var(--global-theme-color);
    background-color: rgba(128, 128, 128, 0.08);
    border: 1px solid rgba(128, 128, 128, 0.14);
  }

  .behbahani-footer-note {
    margin-top: 2rem;
    padding: 1.25rem 1.35rem;
    border-radius: 1rem;
    border: 1px solid var(--card-border);
    background-color: rgba(128, 128, 128, 0.035);
  }

  .behbahani-footer-note p {
    margin: 0;
    line-height: 1.65;
    opacity: 0.86;
  }

  @media (max-width: 900px) {
    .behbahani-grid,
    .behbahani-resource-wrap {
      grid-template-columns: 1fr;
    }

    .behbahani-research-item {
      grid-template-columns: 1fr;
      gap: 0.35rem;
    }
  }

  @media (max-width: 600px) {
    .behbahani-hero {
      padding: 1.55rem 1.25rem;
      border-radius: 1rem;
    }

    .behbahani-hero h2 {
      font-size: 1.55rem;
    }

    .behbahani-card,
    .behbahani-resource,
    .behbahani-highlight,
    .behbahani-footer-note {
      border-radius: 0.85rem;
    }
  }
</style>

<div class="behbahani-page">

  <section class="behbahani-hero">
    <span class="behbahani-kicker">Southwestern Iranian · Syntax · Morphology</span>

    <h2>Behbahani as a window into alignment, stems, and argument structure</h2>

    <p>
      Behbahani is a Southwestern Iranian language spoken primarily in Behbahan, Iran. It is a primarily oral
      language with no standardized writing system and limited descriptive or digital resources. My work on
      Behbahani combines formal syntactic and morphological analysis with documentation-oriented goals, aiming
      to make the language more visible in theoretical linguistics and in computationally usable formats.
    </p>

    <div class="behbahani-tags">
      <span class="behbahani-tag">Split alignment</span>
      <span class="behbahani-tag">Stem alternations</span>
      <span class="behbahani-tag">Agreement</span>
      <span class="behbahani-tag">Voice</span>
      <span class="behbahani-tag">Nominalization</span>
      <span class="behbahani-tag">Language documentation</span>
    </div>
  </section>

  <section class="behbahani-section">
    <h2>Why Behbahani matters</h2>

    <p class="behbahani-section-intro">
      Behbahani is especially important for the study of the syntax-morphology interface because it combines
      complex verbal indexing, split alignment, stem alternations, and the absence of morphological case. This
      combination creates a useful testing ground for theories of agreement, Voice, argument structure, and the
      relation between verbal stems and syntactic structure.
    </p>

    <div class="behbahani-grid">
      <div class="behbahani-card">
        <h3>Alignment without case</h3>
        <p>
          Behbahani shows alignment-sensitive indexing patterns while lacking morphological case, making it useful
          for separating agreement from overt case morphology.
        </p>
      </div>

      <div class="behbahani-card">
        <h3>Stem-sensitive grammar</h3>
        <p>
          Past and non-past stems are not just morphological alternants. They interact with transitivity, aspect,
          non-finite morphology, and argument indexing.
        </p>
      </div>

      <div class="behbahani-card">
        <h3>Underdocumented data</h3>
        <p>
          Because the language has limited published description, careful documentation can contribute both to
          formal theory and to the visibility of minoritized Iranian languages.
        </p>
      </div>
    </div>
  </section>

  <section class="behbahani-section">
    <h2>Research &amp; core puzzles</h2>

    <p class="behbahani-section-intro">
      My dissertation investigates how argument structure, verbal stems, agreement, and alignment interact in
      Behbahani grammar. A central question is whether patterns that appear morphological on the surface are
      better explained through syntactic structure, especially the distribution of Voice and related functional
      projections.
    </p>

    <div class="behbahani-research-list">
      <div class="behbahani-research-item">
        <strong>Split alignment</strong>
        <span>How are subjects and objects indexed across past and non-past environments?</span>
      </div>

      <div class="behbahani-research-item">
        <strong>Stem alternations</strong>
        <span>How do past and non-past stems interact with aspect, transitivity, and non-finite morphology?</span>
      </div>

      <div class="behbahani-research-item">
        <strong>Voice</strong>
        <span>Which syntactic structures license external arguments in different verbal domains?</span>
      </div>

      <div class="behbahani-research-item">
        <strong>Nominalization</strong>
        <span>What do agentive, resultative, and infinitival forms reveal about the size of verbal structure?</span>
      </div>

      <div class="behbahani-research-item">
        <strong>Case and agreement</strong>
        <span>How does the language maintain complex indexing patterns without morphological case?</span>
      </div>
    </div>

    <div class="behbahani-highlight">
      <p>
        As a native speaker and linguistic researcher, I approach Behbahani both as an object of formal analysis
        and as an underdocumented language whose documentation matters beyond theoretical linguistics.
      </p>
    </div>
  </section>

  <section class="behbahani-section">
    <h2>Documentation &amp; computational resources</h2>

    <p class="behbahani-section-intro">
      Because Behbahani has limited publicly available documentation, part of this project is dedicated to creating
      structured resources that can support future descriptive, theoretical, and computational work.
    </p>

    <div class="behbahani-resource-wrap">
      <div class="behbahani-resource">
        <h3>Computational modeling</h3>
        <p>
          I am developing Haskell-based finite-state models to represent selected aspects of Behbahani verbal
          morphology and agreement. These models are intended to make parts of the analysis explicit, testable,
          and reusable.
        </p>
        <span class="status-badge">In progress</span>
      </div>

      <div class="behbahani-resource">
        <h3>Corpus development</h3>
        <p>
          This section will eventually include curated examples, text materials, and grammatical descriptions drawn
          from ongoing fieldwork and native-speaker consultation.
        </p>
        <span class="status-badge">Forthcoming</span>
      </div>
    </div>
  </section>

  <section class="behbahani-section">
    <h2>Related areas</h2>

    <div class="behbahani-grid">
      <div class="behbahani-card">
        <h3>Iranian linguistics</h3>
        <p>
          Behbahani contributes to broader comparative questions about Southwestern Iranian morphosyntax and
          understudied Iranian varieties.
        </p>
      </div>

      <div class="behbahani-card">
        <h3>Syntax-morphology interface</h3>
        <p>
          The project asks how much apparent morphology can be derived from independently motivated syntactic
          structure.
        </p>
      </div>

      <div class="behbahani-card">
        <h3>Language visibility</h3>
        <p>
          A long-term goal is to create resources that make Behbahani more accessible to researchers, students,
          and community-oriented documentation work.
        </p>
      </div>
    </div>
  </section>

  <div class="behbahani-footer-note">
    <p>
      This page will be updated as dissertation chapters, computational models, documentation materials, and
      related presentations become publicly available.
    </p>
  </div>

</div>
