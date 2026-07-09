---
layout: about
title: About
permalink: /
subtitle: PhD Candidate in Linguistics at Stony Brook University

nav: false
news: false
selected_papers: false
social: false
---

<style>
  /* Banner for the default title and subtitle */
  .post-header {
    width: 100% !important;
    max-width: none !important;
    padding: 1.6rem 1.9rem;
    margin: 0.75rem 0 2rem 0;
    border: 1px solid rgba(128, 128, 128, 0.16);
    border-radius: 1.15rem;
    background:
      radial-gradient(
        circle at top right,
        color-mix(in srgb, var(--global-theme-color) 10%, transparent),
        transparent 36%
      ),
      linear-gradient(
        135deg,
        rgba(128, 128, 128, 0.06),
        rgba(128, 128, 128, 0.018)
      );
  }

  .post-header .post-title {
    margin: 0 0 0.45rem 0;
    font-size: clamp(2rem, 4vw, 3rem);
    line-height: 1.05;
    letter-spacing: -0.035em;
  }

  .post-header .post-description {
    margin: 0;
    font-size: 1.05rem;
    line-height: 1.55;
    color: var(--global-theme-color);
    font-weight: 650;
  }

  /* Keep the two columns next to each other */
 .about-layout {
  display: flex;
  flex-direction: row;
  flex-wrap: nowrap;
  align-items: flex-start;
  gap: 2rem;
}

.about-text-col {
  flex: 0 0 60%;
  max-width: 60%;
  line-height: 1.65;
}

.about-photo-col {
  flex: 0 0 32%;
  max-width: 32%;
  border-left: 1px solid rgba(128, 128, 128, 0.16);
  padding-left: 2rem;
  text-align: center;
}

.about-photo-col img {
  width: 100%;
  max-width: 260px;
  margin-bottom: 20px;
}

.about-social-links {
  text-align: left;
  line-height: 2;
  padding-left: 10px;
}
</style>

<div class="about-layout">

<div class="about-text-col" markdown="1">
<p>
  I am a PhD candidate in the Department of Linguistics at Stony Brook University. My research focuses on complex
  alignment systems: what gives rise to them, how apparently complicated agreement patterns are built from
  smaller pieces of grammatical structure, and what theoretical architecture is needed to model them. I pursue
  these questions through Behbahani, a Southwestern Iranian language whose split alignment patterns make these
  mechanisms empirically visible.
</p>
  
<p>
  My dissertation traces how stems, argument indexing, and non-finite forms interact to produce this split,
  treating Behbahani's verbal domain as a case where the architecture behind alignment can be directly examined.
  This work also raises broader questions about the kind of theory needed to model complex agreement systems.
</p>
  
<p>
  Alongside this formal work, I am involved in language documentation and resource-building for underdocumented
  languages, combining fieldwork, corpus development, and computational modeling with theoretical analysis. This
  work is grounded in a broader interest in
  <a href="https://www.unesco.org/en/articles/linguistic-diversity-and-language-rights-power-being-understood" target="_blank" rel="noopener noreferrer">language rights</a>
  and linguistic diversity, and in how
  <a href="https://www.eldp.net/" target="_blank" rel="noopener noreferrer">documentation</a>
  and
  <a href="https://www.elra.info/about/sig/sigul/" target="_blank" rel="noopener noreferrer">language technologies</a>
  can support marginalized and understudied language communities. I am particularly interested in developing
  computational tools and AI more responsibly for languages often left out of mainstream linguistic research and
  technology development.
</p>

<p>
  Beyond my core research, I care about educational equity, particularly what accessibility means inside the
  classroom. To me, accessibility goes beyond financial access: it means designing materials, pedagogy, and
  classroom practices that are genuinely usable by students with different needs. I see this as a shared
  responsibility for instructors and material designers, not only in what we teach, but in how we teach it.
</p>


</div>

<div class="about-photo-col">
  
  <img src="{{ '/assets/img/pardis.jpeg' | relative_url }}" class="img-fluid rounded z-depth-1" alt="Pardis Derakhshandeh">
  
  <div class="about-social-links">
    <i class="fas fa-envelope"></i> <a href="mailto:pardis.derakhshandeh@stonybrook.edu">Email</a><br>
    <i class="fab fa-github"></i> <a href="https://github.com/pardisderakhshandeh">GitHub</a><br>
    <i class="ai ai-google-scholar"></i> <a href="https://scholar.google.com/citations?user=YOUR_SCHOLAR_ID">Google Scholar</a><br>
    <i class="fab fa-linkedin"></i> <a href="https://linkedin.com/in/YOUR_LINKEDIN_ID">LinkedIn</a>
  </div>

</div>

</div>
