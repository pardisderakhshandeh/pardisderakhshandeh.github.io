---
layout: page
title: Research
permalink: /research/
nav: true
nav_order: 2
---

<style>
  .research-page {
    --card-border: rgba(128, 128, 128, 0.16);
    --soft-bg: rgba(128, 128, 128, 0.055);
    --accent-soft: color-mix(in srgb, var(--global-theme-color) 12%, transparent);
  }

  .research-intro {
    padding: 1.65rem 1.75rem;
    margin: 0.5rem 0 2.2rem 0;
    border: 1px solid var(--card-border);
    border-radius: 1.1rem;
    background:
      radial-gradient(circle at top right, var(--accent-soft), transparent 32%),
      linear-gradient(135deg, rgba(128, 128, 128, 0.06), rgba(128, 128, 128, 0.018));
  }

  .research-intro p {
    max-width: 850px;
    margin: 0;
    font-size: 1.02rem;
    line-height: 1.7;
    opacity: 0.88;
  }

  .research-topic {
    margin: 2.1rem 0;
    padding-bottom: 1.4rem;
    border-bottom: 1px solid rgba(128, 128, 128, 0.13);
  }

  .research-topic:last-of-type {
    border-bottom: none;
  }

  .research-topic h2 {
    margin-bottom: 0.65rem;
    font-size: 1.35rem;
  }

  .research-topic p {
    max-width: 850px;
    line-height: 1.68;
    opacity: 0.86;
  }

  .research-topic ul {
    margin-top: 0.85rem;
    padding-left: 1.25rem;
  }

  .research-topic li {
    margin-bottom: 0.5rem;
    line-height: 1.58;
    opacity: 0.86;
  }

  .research-label {
    display: inline-block;
    margin-bottom: 0.75rem;
    padding: 0.25rem 0.65rem;
    border-radius: 999px;
    font-size: 0.72rem;
    font-weight: 700;
    letter-spacing: 0.06em;
    text-transform: uppercase;
    color: var(--global-theme-color);
    background-color: rgba(128, 128, 128, 0.08);
    border: 1px solid rgba(128, 128, 128, 0.14);
  }

  .selected-work {
    margin-top: 2.4rem;
    padding: 1.35rem 1.45rem;
    border-radius: 1rem;
    border: 1px solid var(--card-border);
    background-color: var(--soft-bg);
  }

  .selected-work h2 {
    margin-top: 0;
    margin-bottom: 0.9rem;
  }

  .selected-work ul {
    margin-bottom: 0;
    padding-left: 1.25rem;
  }

  .selected-work li {
    margin-bottom: 0.55rem;
    line-height: 1.58;
  }

  .research-link {
    color: var(--global-theme-color);
    font-weight: 600;
    text-decoration: none;
    border-bottom: 1px solid color-mix(in srgb, var(--global-theme-color) 35%, transparent);
  }

  .research-link:hover {
    color: var(--global-theme-color);
    border-bottom-color: var(--global-theme-color);
    text-decoration: none;
  }

  @media (max-width: 600px) {
    .research-intro,
    .selected-work {
      padding: 1.2rem 1.15rem;
      border-radius: 0.85rem;
    }
  }
</style>

<div class="research-page">

  <div class="research-intro">
    <p>
      My research is in syntax and morphology, with a focus on how surface morphological patterns reveal the
      structure of clauses, verbal domains, and nominalized expressions. I work primarily on Iranian languages,
      especially Behbahani, and I am interested in how data from underdocumented languages can sharpen broader
      theoretical questions about argument structure, agreement, and the syntax-morphology interface.
    </p>
  </div>

  <section class="research-topic">
    <span class="research-label">Research area</span>
    <h2>Verbal structure and morphological form</h2>

    <p>
      One strand of my research asks how verbal morphology reflects syntactic structure. I am especially interested
      in cases where stem choice, tense/aspect morphology, and verbal derivation are not independent pieces of
      morphology, but instead track the size and composition of the verbal domain.
    </p>

    <p>
      In my work on Behbahani, this question becomes central because past and non-past stems interact with
      transitivity, agreement, and non-finite morphology in ways that suggest a close relationship between stem
      formation and syntactic structure.
    </p>
  </section>

  <section class="research-topic">
    <span class="research-label">Research area</span>
    <h2>Argument indexing without morphological case</h2>

    <p>
      A second strand of my research investigates how languages organize subject and object indexing when overt
      case morphology is absent. This is theoretically useful because it allows agreement and alignment to be
      studied without assuming that case marking is doing the explanatory work.
    </p>

    <p>
      Behbahani provides an important empirical domain for this question: argument indexing is sensitive to verbal
      environment and argument expression, even though the language does not mark arguments with morphological case.
    </p>
  </section>

  <section class="research-topic">
    <span class="research-label">Research area</span>
    <h2>Nominalization and non-finite structure</h2>

    <p>
      I also study nominalized and non-finite forms as diagnostics for verbal structure. Agentive, resultative, and
      infinitival forms can reveal how much verbal structure is present below the nominal layer, and whether
      argument-introducing structure is available in a given domain.
    </p>

    <p>
      This part of my work connects the analysis of individual morphological forms to larger questions about Voice,
      argument introduction, and the boundary between verbal and nominal structure.
    </p>
  </section>

  <section class="research-topic">
    <span class="research-label">Research area</span>
    <h2>Underdocumented Iranian languages and formal theory</h2>

    <p>
      My research is also shaped by a commitment to bringing underdocumented Iranian languages into formal
      linguistic theory. I treat documentation and theoretical analysis as mutually reinforcing: careful empirical
      description creates the foundation for formal argumentation, while theoretical questions help identify which
      patterns require deeper documentation.
    </p>

    <p>
      For a general introduction to Behbahani, see the
      <a class="research-link" href="/behbahani/">Behbahani</a> page. For specific ongoing projects, including
      computational modeling and corpus development, see the
      <a class="research-link" href="/projects/">Projects</a> page.
    </p>
  </section>

  <section class="selected-work">
    <h2>Selected current work</h2>

    <ul>
      <li>
        <strong>Dissertation:</strong> syntax and morphology of Behbahani verbal structure, with a focus on
        stem choice, argument indexing, and non-finite domains.
      </li>
      <li>
        <strong>Conference work:</strong> selectional restrictions on Voice and stem-driven split alignment in
        Behbahani.
      </li>
      <li>
        <strong>Ongoing work:</strong> documentation, corpus development, and computational modeling of selected
        aspects of Behbahani agreement and verbal morphology.
      </li>
    </ul>
  </section>

</div>
