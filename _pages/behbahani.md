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

  .language-hero {
    padding: 2.2rem 2rem;
    margin: 0.5rem 0 2.4rem 0;
    border: 1px solid var(--card-border);
    border-radius: 1.35rem;
    background:
      radial-gradient(circle at top right, var(--accent-soft), transparent 34%),
      linear-gradient(135deg, rgba(128, 128, 128, 0.07), rgba(128, 128, 128, 0.02));
  }

  .language-kicker {
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

  .language-hero h2 {
    margin: 0 0 0.85rem 0;
    font-size: clamp(1.65rem, 3vw, 2.35rem);
    line-height: 1.15;
    letter-spacing: -0.02em;
  }

  .language-hero p {
    max-width: 800px;
    margin-bottom: 0;
    font-size: 1.02rem;
    line-height: 1.68;
    opacity: 0.88;
  }

  .language-tags {
    display: flex;
    flex-wrap: wrap;
    gap: 0.45rem;
    margin-top: 1.35rem;
  }

  .language-tag {
    display: inline-block;
    padding: 0.28rem 0.7rem;
    border-radius: 999px;
    font-size: 0.78rem;
    font-weight: 600;
    color: var(--global-text-color);
    background-color: var(--global-bg-color);
    border: 1px solid var(--card-border);
  }

  .language-section {
    margin: 2.35rem 0;
  }

  .language-section h2 {
    margin-bottom: 0.75rem;
  }

  .section-intro {
    max-width: 820px;
    margin-bottom: 1.25rem;
    line-height: 1.65;
    opacity: 0.84;
  }

  .profile-grid {
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));
    gap: 1rem;
    margin-top: 1.25rem;
  }

  .profile-card {
    padding: 1.1rem 1.15rem;
    border: 1px solid var(--card-border);
    border-radius: 1rem;
    background-color: var(--softer-bg);
  }

  .profile-card h3 {
    margin: 0 0 0.45rem 0;
    font-size: 0.78rem;
    text-transform: uppercase;
    letter-spacing: 0.06em;
    color: var(--global-theme-color);
  }

  .profile-card p {
    margin: 0;
    font-size: 0.94rem;
    line-height: 1.55;
    opacity: 0.86;
  }

  .feature-list {
    display: grid;
    grid-template-columns: 1fr;
    gap: 0.8rem;
    margin-top: 1.25rem;
  }

  .feature-item {
    display: grid;
    grid-template-columns: 12rem 1fr;
    gap: 1rem;
    padding: 1rem 1.1rem;
    border: 1px solid var(--card-border);
    border-radius: 0.95rem;
    background-color: rgba(128, 128, 128, 0.03);
  }

  .feature-item strong {
    color: var(--global-theme-color);
  }

  .feature-item span {
    line-height: 1.58;
    opacity: 0.86;
  }

  .language-note {
    padding: 1.25rem 1.35rem;
    margin: 1.6rem 0;
    border-left: 4px solid var(--global-theme-color);
    border-radius: 0.85rem;
    background-color: var(--soft-bg);
  }

  .language-note p {
    margin: 0;
    line-height: 1.65;
    opacity: 0.88;
  }

  .resource-grid {
    display: grid;
    grid-template-columns: repeat(2, minmax(0, 1fr));
    gap: 1rem;
    margin-top: 1.25rem;
  }

  .resource-card {
    padding: 1.2rem;
    border: 1px solid var(--card-border);
    border-radius: 1rem;
    background:
      linear-gradient(180deg, rgba(128, 128, 128, 0.055), rgba(128, 128, 128, 0.02));
  }

  .resource-card h3 {
    margin-top: 0;
    margin-bottom: 0.5rem;
    font-size: 1rem;
  }

  .resource-card p {
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

  .language-link {
    color: var(--global-theme-color);
    font-weight: 600;
    text-decoration: none;
    border-bottom: 1px solid color-mix(in srgb, var(--global-theme-color) 35%, transparent);
  }

  .language-link:hover {
    color: var(--global-theme-color);
    border-bottom-color: var(--global-theme-color);
    text-decoration: none;
  }

  @media (max-width: 900px) {
    .profile-grid,
    .resource-grid {
      grid-template-columns: 1fr;
    }

    .feature-item {
      grid-template-columns: 1fr;
      gap: 0.35rem;
    }
  }

  @media (max-width: 600px) {
    .language-hero {
      padding: 1.55rem 1.25rem;
      border-radius: 1rem;
    }

    .language-hero h2 {
      font-size: 1.55rem;
    }

    .profile-card,
    .resource-card,
    .language-note {
      border-radius: 0.85rem;
    }
  }
</style>

<div class="behbahani-page">

  <section class="language-hero">
    <span class="language-kicker">About Behbahani</span>

    <h2>A Southwestern Iranian language from Behbahan, Iran</h2>

    <p>
      Behbahani is a Southwestern Iranian language spoken primarily in Behbahan, in southwestern Iran.
      It is a primarily oral language with no standardized writing system and limited publicly available
      linguistic resources. This page provides a brief overview of the language, its grammatical profile,
      and ongoing work to document and analyze it.
    </p>

    <div class="language-tags">
      <span class="language-tag">Southwestern Iranian</span>
      <span class="language-tag">Primarily oral</span>
      <span class="language-tag">Underdocumented</span>
      <span class="language-tag">No standard orthography</span>
      <span class="language-tag">Syntax</span>
      <span class="language-tag">Morphology</span>
    </div>
  </section>

  <section class="language-section">
    <h2>Language profile</h2>

    <p class="section-intro">
      Behbahani belongs to the Iranian branch of the Indo-Iranian languages. It is used as a local and community
      language in and around Behbahan, while Persian is the dominant language of education, administration, media,
      and public writing.
    </p>

    <div class="profile-grid">
      <div class="profile-card">
        <h3>Family</h3>
        <p>Indo-European, Indo-Iranian, Iranian, Southwestern Iranian.</p>
      </div>

      <div class="profile-card">
        <h3>Location</h3>
        <p>Primarily associated with Behbahan, in southwestern Iran.</p>
      </div>

      <div class="profile-card">
        <h3>Writing</h3>
        <p>Primarily oral, with no widely standardized orthography.</p>
      </div>

      <div class="profile-card">
        <h3>Status</h3>
        <p>Underdocumented, with limited descriptive and digital resources.</p>
      </div>

      <div class="profile-card">
        <h3>Research value</h3>
        <p>A useful case for studying agreement, alignment, stems, and argument structure.</p>
      </div>

      <div class="profile-card">
        <h3>Documentation</h3>
        <p>Ongoing work includes elicited data, naturalistic speech, and syntactic annotation.</p>
      </div>
    </div>
  </section>

  <section class="language-section">
    <h2>Grammatical features at a glance</h2>

    <p class="section-intro">
      Behbahani is especially interesting for formal linguistics because several core grammatical patterns interact
      in ways that are not immediately visible from surface word forms alone. My work focuses on how these patterns
      can be analyzed at the syntax-morphology interface.
    </p>

    <div class="feature-list">
      <div class="feature-item">
        <strong>Pro-drop</strong>
        <span>Subjects can often be omitted when their reference is recoverable from verbal morphology and context.</span>
      </div>

      <div class="feature-item">
        <strong>No morphological case</strong>
        <span>The language does not mark arguments with overt morphological case, which makes its indexing patterns theoretically important.</span>
      </div>

      <div class="feature-item">
        <strong>Split alignment</strong>
        <span>Argument indexing differs across past and non-past environments, creating a split alignment pattern.</span>
      </div>

      <div class="feature-item">
        <strong>Stem alternations</strong>
        <span>Past and non-past stems interact with tense, aspect, transitivity, and non-finite morphology.</span>
      </div>

      <div class="feature-item">
        <strong>Agreement patterns</strong>
        <span>Subject and object indexing are sensitive to tense, transitivity, and whether certain arguments are overtly expressed.</span>
      </div>

      <div class="feature-item">
        <strong>Nominalization</strong>
        <span>Agentive, resultative, and infinitival forms provide evidence about the size and structure of verbal domains.</span>
      </div>
    </div>
  </section>

  <section class="language-section">
    <h2>Why Behbahani matters</h2>

    <p class="section-intro">
      Behbahani matters for two connected reasons. Empirically, it is an underdocumented Iranian language whose
      grammar has not been fully represented in the descriptive or digital record. Theoretically, it provides
      evidence for how agreement, Voice, stem formation, and argument structure interact in a language without
      overt morphological case.
    </p>

    <div class="language-note">
      <p>
        As a native speaker and linguistic researcher, I approach Behbahani both as a language that deserves
        documentation and as a grammatical system that can contribute to broader debates in syntax and morphology.
      </p>
    </div>
  </section>

  <section class="language-section">
    <h2>Documentation and resources</h2>

    <p class="section-intro">
      This section will grow as documentation materials, computational models, and annotated data become available.
      The long-term goal is to create resources that are useful for researchers, students, and community-oriented
      language documentation.
    </p>

    <div class="resource-grid">
      <div class="resource-card">
        <h3>Grammar notes</h3>
        <p>
          Short descriptions of core grammatical patterns, including agreement, alignment, stems, and nominalization.
        </p>
        <span class="status-badge">Forthcoming</span>
      </div>

      <div class="resource-card">
        <h3>Glossed examples</h3>
        <p>
          Curated examples with transliteration, glossing, and translation, drawn from elicitation and fieldwork.
        </p>
        <span class="status-badge">Forthcoming</span>
      </div>

      <div class="resource-card">
        <h3>Computational models</h3>
        <p>
          Haskell-based finite-state models for selected aspects of Behbahani agreement and verbal morphology.
        </p>
        <span class="status-badge">In progress</span>
      </div>

      <div class="resource-card">
        <h3>Corpus and treebank</h3>
        <p>
          A developing corpus and syntactically annotated dataset designed for future descriptive, theoretical,
          and computational work.
        </p>
        <span class="status-badge">In progress</span>
      </div>
    </div>
  </section>

  <section class="language-section">
    <h2>Related work</h2>

    <p class="section-intro">
      My broader research on Behbahani investigates the syntax-morphology interface, especially split alignment,
      verbal stems, agreement, Voice, and nominalization. More information about these projects is available on
      the <a class="language-link" href="/projects/">Projects</a> and <a class="language-link" href="/research/">Research</a> pages.
    </p>
  </section>

</div>
