---
layout: page
title: Projects
permalink: /projects/
nav: true
nav_order: 4
---

<style>
  .projects-page {
    --card-border: rgba(128, 128, 128, 0.16);
    --soft-bg: rgba(128, 128, 128, 0.055);
    --softer-bg: rgba(128, 128, 128, 0.035);
    --accent-soft: color-mix(in srgb, var(--global-theme-color) 12%, transparent);
  }

  .projects-hero {
    padding: 2.1rem 2rem;
    margin: 0.5rem 0 2.3rem 0;
    border: 1px solid var(--card-border);
    border-radius: 1.35rem;
    background:
      radial-gradient(circle at top right, var(--accent-soft), transparent 34%),
      linear-gradient(135deg, rgba(128, 128, 128, 0.07), rgba(128, 128, 128, 0.02));
  }

  .projects-kicker {
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

  .projects-hero h2 {
    margin: 0 0 0.85rem 0;
    font-size: clamp(1.65rem, 3vw, 2.3rem);
    line-height: 1.15;
    letter-spacing: -0.02em;
  }

  .projects-hero p {
    max-width: 790px;
    margin-bottom: 0;
    font-size: 1.02rem;
    line-height: 1.68;
    opacity: 0.88;
  }

  .project-grid {
    display: grid;
    grid-template-columns: 1fr;
    gap: 1.25rem;
  }

  .project-card {
    position: relative;
    padding: 1.45rem 1.55rem;
    border: 1px solid var(--card-border);
    border-radius: 1.1rem;
    background:
      linear-gradient(180deg, rgba(128, 128, 128, 0.052), rgba(128, 128, 128, 0.018));
    transition: transform 160ms ease, border-color 160ms ease, background-color 160ms ease;
  }

  .project-card:hover {
    transform: translateY(-2px);
    border-color: rgba(128, 128, 128, 0.26);
    background-color: var(--soft-bg);
  }

  .project-card-header {
    display: flex;
    align-items: flex-start;
    justify-content: space-between;
    gap: 1rem;
    margin-bottom: 0.75rem;
  }

  .project-card h2 {
    margin: 0;
    font-size: 1.25rem;
    line-height: 1.3;
  }

  .project-status {
    flex: 0 0 auto;
    display: inline-block;
    padding: 0.28rem 0.68rem;
    border-radius: 999px;
    font-size: 0.72rem;
    font-weight: 700;
    letter-spacing: 0.04em;
    text-transform: uppercase;
    color: var(--global-theme-color);
    background-color: rgba(128, 128, 128, 0.08);
    border: 1px solid rgba(128, 128, 128, 0.14);
    white-space: nowrap;
  }

  .project-card p {
    margin-bottom: 0.9rem;
    line-height: 1.65;
    opacity: 0.86;
  }

  .project-card ul {
    margin: 0.85rem 0 0 0;
    padding-left: 1.25rem;
  }

  .project-card li {
    margin-bottom: 0.55rem;
    line-height: 1.58;
    opacity: 0.86;
  }

  .project-card li:last-child {
    margin-bottom: 0;
  }

  .project-tags {
    display: flex;
    flex-wrap: wrap;
    gap: 0.45rem;
    margin-top: 1rem;
  }

  .project-tag {
    display: inline-block;
    padding: 0.25rem 0.62rem;
    border-radius: 999px;
    font-size: 0.75rem;
    font-weight: 600;
    color: var(--global-text-color);
    background-color: var(--global-bg-color);
    border: 1px solid var(--card-border);
  }

  .project-link {
    color: var(--global-theme-color);
    font-weight: 600;
    text-decoration: none;
    border-bottom: 1px solid color-mix(in srgb, var(--global-theme-color) 35%, transparent);
  }

  .project-link:hover {
    color: var(--global-theme-color);
    border-bottom-color: var(--global-theme-color);
    text-decoration: none;
  }

  @media (max-width: 700px) {
    .projects-hero {
      padding: 1.55rem 1.25rem;
      border-radius: 1rem;
    }

    .project-card {
      padding: 1.2rem 1.2rem;
    }

    .project-card-header {
      flex-direction: column;
      gap: 0.55rem;
    }

    .project-status {
      align-self: flex-start;
    }
  }
</style>

<div class="projects-page">

  <section class="projects-hero">
    <span class="projects-kicker">Research projects · Documentation · Computational modeling</span>

    <h2>Projects at the intersection of theory, documentation, and computation</h2>

    <p>
      My current projects center on Behbahani, an underdocumented Southwestern Iranian language. These projects
      connect formal syntactic analysis with computational modeling, corpus development, syntactic annotation,
      and collaborative language documentation.
    </p>
  </section>

  <div class="project-grid">

    <section class="project-card">
      <div class="project-card-header">
        <h2>Computational Modeling of Behbahani Agreement</h2>
        <span class="project-status">In progress</span>
      </div>

      <p>
        To complement my theoretical syntactic analysis, I am developing computational models that formally
        represent selected aspects of Behbahani agreement and alignment.
      </p>

      <ul>
        <li>
          Developing finite-state automata using Haskell to model interactions among tense, transitivity,
          stem choice, and agreement in a system without morphological case.
        </li>
        <li>
          Using functional programming as a way to make the analysis explicit, testable, and easier to compare
          with alternative accounts of split alignment.
        </li>
      </ul>
    </section>

    <section class="project-card">
      <div class="project-card-header">
        <h2>Behbahani Corpus and Syntactic Treebank</h2>
        <span class="project-status">In progress</span>
      </div>

      <p>
        To establish a durable empirical foundation for future research on Behbahani, I am developing a digitized
        corpus and a custom syntactically annotated treebank.
      </p>

      <ul>
        <li>
          Compiling a foundational textual corpus based on elicited data, naturalistic speech recordings, and
          fieldwork materials.
        </li>
        <li>
          Designing a theoretically informed syntactic annotation scheme tailored to Behbahani morphosyntax,
          including agreement patterns, stem alternations, and argument-structure distinctions.
        </li>
      </ul>
    </section>

    <section class="project-card">
      <div class="project-card-header">
        <h2>Language Documentation and Mentorship: Linguists, Meet Behbahani</h2>
        <span class="project-status">2024-2025</span>
      </div>

      <p>
        Beyond formal analysis, I am invested in the documentation and visibility of Behbahani. This project grew
        out of fieldwork data collected in the LIN 431 fieldwork course, where I served as linguistic consultant
        and teaching assistant.
      </p>

      <ul>
        <li>
          Co-directed a collaborative documentation initiative with
          <a class="project-link" href="https://www.danielgreeson.com/home" target="_blank" rel="noopener noreferrer">Daniel Greeson</a>,
          using primary data elicited through the LIN 431 fieldwork course.
        </li>
        <li>
          Selected and mentored a team of ten undergraduate researchers from May 2024 through January 2025,
          guiding the transformation of raw fieldwork data into developed research projects.
        </li>
        <li>
          Developed the project as a bridge between language documentation, undergraduate research training,
          and formal analysis of an underdocumented Iranian language.
        </li>
      </ul>
    </section>

  </div>

</div>
