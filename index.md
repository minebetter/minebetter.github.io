---
layout: default
permalink: /
---

<div class="home">
  <section class="hero">
    <p class="hero-kicker">{{ site.profile.role }} · {{ site.profile.department }}</p>
    <h1>{{ site.profile.name }}</h1>
    <p class="hero-lead">{{ site.profile.bio }}</p>

    <div class="hero-meta">
      {% for interest in site.profile.interests %}
      <span class="chip">{{ interest }}</span>
      {% endfor %}
    </div>

    <div class="hero-links">
      <a class="button-link" href="mailto:{{ site.profile.email }}">Email</a>
      <a class="button-link secondary" href="https://github.com/{{ site.profile.github }}">GitHub</a>
    </div>
  </section>

  <div class="home-grid">
    <div class="stack">
      <section class="panel">
        <h2>About</h2>
        <p>I am a Ph.D. student at {{ site.profile.institution }}, where I work on natural language processing, reasoning, and the evaluation of large language models. My recent interests include multimodal generation, chain-of-thought analysis, and building reliable AI systems that remain useful under real-world constraints.</p>
        <p>Before joining CUHK, I received my B.Eng. in Electronic Information Science and Technology from Tsinghua University in 2025.</p>
      </section>

      <section class="panel">
        <h2>Selected Work</h2>
        <article class="publication">
          <h3>From Broad Exploration to Stable Synthesis: Entropy-Guided Optimization for Autoregressive Image Generation</h3>
          <p class="meta-line">Han Song, Yucheng Zhou, Jianbing Shen, Yu Cheng · ICLR 2026 Poster</p>
          <p><a href="https://iclr.cc/virtual/2026/poster/10009885">Paper page</a></p>
        </article>
      </section>

      <section class="panel">
        <h2>Experience</h2>
        <div class="timeline">
          <article class="timeline-item">
            <h3>Shanghai AI Laboratory</h3>
            <p class="meta-line">Research Intern · Jul 2024 - Jul 2025</p>
            <ul class="highlights-list">
              <li>Worked on inference acceleration for autoregressive video generation.</li>
              <li>Studied hybrid Mamba-GPT architectures to balance generation quality and efficiency.</li>
              <li>Explored multi-agent customized video generation with subject consistency modeling.</li>
            </ul>
          </article>
        </div>
      </section>
    </div>

    <div class="stack">
      <section class="panel">
        <h2>Education</h2>
        <div class="timeline">
          <article class="timeline-item">
            <h3>The Chinese University of Hong Kong</h3>
            <p class="meta-line">Ph.D. in Computer Science and Engineering · Sep 2025 - Present</p>
            <p>{{ site.profile.location }}</p>
          </article>
          <article class="timeline-item">
            <h3>Tsinghua University</h3>
            <p class="meta-line">B.Eng. in Electronic Information Science and Technology · Sep 2020 - Jun 2025</p>
            <p>Beijing, China · GPA: 3.9/4.0</p>
          </article>
        </div>
      </section>

      <section class="panel">
        <h2>Honors and Awards</h2>
        <ul class="highlights-list">
          <li>Outstanding Graduate, Tsinghua University (Jun 2025)</li>
          <li>Comprehensive Excellence Award, Academic Excellence Award, and Science and Technology Innovation Award (2021 - 2024)</li>
        </ul>
      </section>

      <section class="panel">
        <h2>Contact</h2>
        <ul class="contact-list">
          <li>Email: <a href="mailto:{{ site.profile.email }}">{{ site.profile.email }}</a></li>
          {% if site.profile.gmail and site.profile.gmail != "" %}
          <li>Gmail: <a href="mailto:{{ site.profile.gmail }}">{{ site.profile.gmail }}</a></li>
          {% endif %}
          <li>GitHub: <a href="https://github.com/{{ site.profile.github }}">@{{ site.profile.github }}</a></li>
          <li>Institution: {{ site.profile.institution }}</li>
        </ul>
      </section>
    </div>
  </div>
</div>
