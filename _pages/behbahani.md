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
    max-width: 850px;
    margin-bottom: 0;
    font-size: 1.02rem;
    line-height: 1.68;
    opacity: 0.88;
  }

  .language-section {
    margin: 2.35rem 0;
  }

  .language-section h2 {
    margin-bottom: 0.75rem;
  }

  .section-intro {
    max-width: 850px;
    margin-bottom: 1.25rem;
    line-height: 1.65;
    opacity: 0.84;
  }

  .quick-facts {
    display: grid;
    grid-template-columns: 14rem 1fr;
    border: 1px solid var(--card-border);
    border-radius: 1rem;
    overflow: hidden;
    background-color: var(--softer-bg);
  }

  .quick-facts div {
    padding: 0.85rem 1rem;
    border-bottom: 1px solid var(--card-border);
  }

  .quick-facts div:nth-child(odd) {
    font-weight: 700;
    color: var(--global-theme-color);
    background-color: rgba(128, 128, 128, 0.045);
  }

  .quick-facts div:nth-last-child(-n + 2) {
    border-bottom: none;
  }

  .map-placeholder,
  .audio-placeholder,
  .example-card,
  .language-note {
    padding: 1.25rem 1.35rem;
    margin: 1.6rem 0;
    border: 1px solid var(--card-border);
    border-radius: 1rem;
    background-color: var(--soft-bg);
  }

  .map-placeholder {
    min-height: 230px;
    display: flex;
    align-items: center;
    justify-content: center;
    text-align: center;
  }

  .map-placeholder p,
  .audio-placeholder p,
  .language-note p {
    margin: 0;
    line-height: 1.65;
    opacity: 0.88;
  }

  .profile-grid,
  .resource-grid {
    display: grid;
    grid-template-columns: repeat(2, minmax(0, 1fr));
    gap: 1rem;
    margin-top: 1.25rem;
  }

  .profile-card,
  .resource-card {
    padding: 1.15rem 1.2rem;
    border: 1px solid var(--card-border);
    border-radius: 1rem;
    background:
      linear-gradient(180deg, rgba(128, 128, 128, 0.055), rgba(128, 128, 128, 0.02));
  }

  .profile-card h3,
  .resource-card h3 {
    margin-top: 0;
    margin-bottom: 0.5rem;
    font-size: 1rem;
  }

  .profile-card p,
  .resource-card p {
    margin: 0;
    font-size: 0.94rem;
    line-height: 1.58;
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
    border-left: 4px solid var(--global-theme-color);
  }

  .status-badge {
    display: inline-block;
    margin-top: 0.85rem;
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

  .example-card pre {
    margin: 0;
    white-space: pre-wrap;
    font-size: 0.92rem;
    line-height: 1.6;
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

    .feature-item,
    .quick-facts {
      grid-template-columns: 1fr;
    }

    .quick-facts div:nth-child(odd) {
      padding-bottom: 0.25rem;
    }

    .quick-facts div:nth-child(even) {
      padding-top: 0.25rem;
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
  }
</style>

<div class="behbahani-page">

  <section class="language-hero">
    <span class="language-kicker">About Behbahani</span>

    <h2>An underdocumented Southwestern Iranian language from Behbahan, Iran</h2>

    <p>
      Behbahani is a Southwestern Iranian language spoken primarily in and around Behbahan, in southwestern Iran.
      Although it is historically related to Persian, it has its own grammatical profile, including distinctive
      patterns of agreement, argument indexing, stem alternations, and nominalization. This page introduces the
      language, its linguistic profile, and ongoing work to document and analyze it.
    </p>
  </section>

  <section class="language-section">
    <h2>Quick facts</h2>

    <div class="quick-facts">
      <div>Language</div>
      <div>Behbahani</div>

      <div>Family</div>
      <div>Indo-European, Indo-Iranian, Iranian, Southwestern Iranian</div>

      <div>Region</div>
      <div>Behbahan, Khuzestan Province, Iran</div>

      <div>Writing system</div>
      <div>No widely standardized orthography</div>

      <div>Primary public language</div>
      <div>Persian is dominant in education, administration, media, and public writing</div>

      <div>Documentation status</div>
      <div>Underdocumented, with limited publicly available linguistic resources</div>

      <div>Research relevance</div>
      <div>Agreement, split alignment, verbal stems, nominalization, and the syntax-morphology interface</div>
    </div>
  </section>

  <section class="language-section">
    <h2>Location</h2>

    <p class="section-intro">
      Behbahani is associated with Behbahan, a city in Khuzestan Province in southwestern Iran. A map will be added
      here to show the location of Behbahan within Iran and its relation to neighboring regions and Iranian languages.
    </p>

    <div class="map-placeholder">
      <p>
        <strong>Map placeholder</strong><br>
        Add a map of Behbahan, Khuzestan, Iran here.
      </p>
    </div>
  </section>

  <section class="language-section">
    <h2>Why Behbahani matters</h2>

    <p class="section-intro">
      Behbahani matters both empirically and theoretically. Empirically, it is an underdocumented Iranian language
      whose grammar has not been fully represented in the descriptive or digital record. Theoretically, it offers
      important evidence for how complex agreement and alignment systems are built, especially in a language without
      overt morphological case.
    </p>

    <div class="profile-grid">
      <div class="profile-card">
        <h3>Iranian linguistics</h3>
        <p>
          Behbahani contributes to the study of Southwestern Iranian languages and helps document grammatical
          diversity within the Iranian language family.
        </p>
      </div>

      <div class="profile-card">
        <h3>Agreement and alignment</h3>
        <p>
          Its agreement patterns make it possible to study split alignment without relying on overt case morphology.
        </p>
      </div>

      <div class="profile-card">
        <h3>Morphology and stems</h3>
        <p>
          The interaction of past and non-past stems with verbal morphology offers evidence for the structure of
          verbal domains.
        </p>
      </div>

      <div class="profile-card">
        <h3>Documentation and technology</h3>
        <p>
          Work on Behbahani can support language documentation, digital resources, and computational modeling for
          underrepresented languages.
        </p>
      </div>
    </div>

    <div class="language-note">
      <p>
        As a native speaker and linguistic researcher, I approach Behbahani both as a language that deserves
        documentation and as a grammatical system that can contribute to broader debates in syntax and morphology.
      </p>
    </div>
  </section>

  <section class="language-section">
    <h2>Language profile</h2>

    <p class="section-intro">
      Behbahani is used as a local and community language in and around Behbahan, while Persian functions as the
      dominant language of formal education, administration, media, and most written communication. Like many
      underdocumented languages, Behbahani is primarily transmitted through speech and everyday community use rather
      than through standardized schooling or public writing.
    </p>

    <div class="profile-grid">
      <div class="profile-card">
        <h3>Community use</h3>
        <p>
          Behbahani is primarily used in local, family, and community contexts. More detailed sociolinguistic
          information will be added as documentation develops.
        </p>
      </div>

      <div class="profile-card">
        <h3>Orality</h3>
        <p>
          The language is primarily oral and does not currently have a widely standardized spelling system.
        </p>
      </div>

      <div class="profile-card">
        <h3>Contact with Persian</h3>
        <p>
          Behbahani exists alongside Persian, which shapes literacy, schooling, media exposure, and public language use.
        </p>
      </div>

      <div class="profile-card">
        <h3>Documentation</h3>
        <p>
          Current work includes elicitation, grammatical description, naturalistic speech data, and syntactic analysis.
        </p>
      </div>
    </div>
  </section>

  <section class="language-section">
    <h2>Grammatical sketch</h2>

    <p class="section-intro">
      Behbahani has several grammatical properties that make it valuable for descriptive, theoretical, and
      computational work. The points below provide a brief overview. Fuller descriptions and examples will be added
      as this page develops.
    </p>

    <div class="feature-list">
      <div class="feature-item">
        <strong>Pro-drop</strong>
        <span>Subjects can often be omitted when their reference is recoverable from verbal morphology and context.</span>
      </div>

      <div class="feature-item">
        <strong>No overt case marking</strong>
        <span>Arguments are not marked by overt morphological case, which makes the language especially useful for studying indexing and alignment.</span>
      </div>

      <div class="feature-item">
        <strong>Split alignment</strong>
        <span>Argument indexing differs across past and non-past environments, producing a split alignment pattern.</span>
      </div>

      <div class="feature-item">
        <strong>Agreement patterns</strong>
        <span>Subject and object indexing are sensitive to tense, transitivity, and whether arguments are overtly expressed.</span>
      </div>

      <div class="feature-item">
        <strong>Stem alternations</strong>
        <span>Past and non-past stems interact with tense, aspect, transitivity, causation, and non-finite morphology.</span>
      </div>

      <div class="feature-item">
        <strong>Nominalization</strong>
        <span>Agentive, resultative, and infinitival forms provide evidence about the size and structure of verbal domains.</span>
      </div>
    </div>
  </section>

  <section class="language-section">
    <h2>Sample text</h2>

    <p class="section-intro">
      Glossed examples will be added here to illustrate Behbahani phonology, morphology, agreement, and syntax.
    </p>

    <div class="example-card">
      <pre><strong>Example placeholder</strong>

Behbahani:
[Add Behbahani sentence here.]

Transliteration:
[Add transliteration here.]

Gloss:
[Add morpheme-by-morpheme gloss here.]

Translation:
[Add English translation here.]</pre>
    </div>
  </section>

  <section class="language-section">
    <h2>Audio</h2>

    <p class="section-intro">
      Short audio samples will be added here in the future, including words, sentences, and short naturalistic speech
      excerpts where appropriate.
    </p>

    <div class="audio-placeholder">
      <p>
        <strong>Audio placeholder</strong><br>
        Add audio samples here later, for example word lists, short sentences, or a brief spoken passage.
      </p>
    </div>
  </section>

  <section class="language-section">
    <h2>Documentation and resources</h2>

    <p class="section-intro">
      This section tracks current and future resources for Behbahani. The long-term goal is to create materials that
      are useful for researchers, students, and community-oriented language documentation.
    </p>

    <div class="resource-grid">
      <div class="resource-card">
        <h3>Current documentation</h3>
        <p>
          Elicited data, agreement paradigms, verbal stems, nominalization patterns, and syntactic examples.
        </p>
        <span class="status-badge">Current</span>
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
          Computational models for selected aspects of Behbahani agreement and verbal morphology.
        </p>
        <span class="status-badge">In progress</span>
      </div>

      <div class="resource-card">
        <h3>Corpus and annotation</h3>
        <p>
          A developing corpus and syntactically annotated dataset designed for future descriptive, theoretical,
          and computational work.
        </p>
        <span class="status-badge">In progress</span>
      </div>
    </div>
  </section>

  <section class="language-section">
    <h2>References and further reading</h2>

  <section class="language-section">
    <h2>Related work</h2>

    <p class="section-intro">
      This page is a companion to my broader research on the syntax-morphology interface. For the theoretical
      framing of this work and current projects, see the <a class="language-link" href="/projects/">Projects</a>
      and <a class="language-link" href="/research/">Research</a> pages.
    </p>
  </section>

</div>
