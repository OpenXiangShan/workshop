---
layout: default
title: Home
description: Call for papers for the 1st Workshop on Agile Development and Verification for Chips at MICRO 2026.
---

{% assign workshop = site.data.workshop %}

<section class="hero" id="top">
  <div class="hero-inner">
    <div class="hero-copy">
      <p class="eyebrow"><span></span>{{ workshop.conference }} Workshop</p>
      <h1>{{ workshop.acronym }} <em>2026</em></h1>
      <p class="hero-title">{{ workshop.title }}</p>
      <p class="hero-summary">A focused forum on agile chip development, rigorous verification, and the tools that make both possible.</p>
      <div class="hero-actions">
        <a class="button button-accent" href="{{ '/cfp/' | relative_url }}">View the call for papers <span aria-hidden="true">↗</span></a>
        <a class="text-link" href="#about">Explore the workshop <span aria-hidden="true">↓</span></a>
      </div>
    </div>
    <div class="hero-index" aria-hidden="true">
      <span>01</span>
      <span>AGILE</span>
      <span>VERIFY</span>
      <span>CHIPS</span>
    </div>
  </div>
  <dl class="event-strip" aria-label="Workshop information">
    <div><dt>Date</dt><dd>{{ workshop.date }}</dd></div>
    <div><dt>Location</dt><dd>{{ workshop.location }}</dd></div>
    <div><dt>Format</dt><dd>{{ workshop.duration }} · {{ workshop.expected_attendance }}</dd></div>
    <div><dt>Presented at</dt><dd><a href="{{ workshop.micro_workshops_url }}" target="_blank" rel="noreferrer">{{ workshop.conference }} <span aria-hidden="true">↗</span></a></dd></div>
  </dl>
</section>

<section class="section about" id="about">
  <div class="section-heading">
    <p class="section-kicker">01 / About</p>
    <h2>Chip design is changing.<br>Verification must keep up.</h2>
  </div>
  <div class="reading-width lead-copy">
    <p class="lede">Agile development and verification for reliable chips.</p>
    <p>In the era of intelligence, AI applications, especially large language models and agents, create computing demands that are increasingly complex, diverse, and fragmented. Customized chips are increasingly necessary, but traditional design tools, labor, and IP costs, together with long design cycles, cannot keep pace with changing demands.</p>
    <p>The hardware community is responding with agile development and verification methodologies. Community-driven products such as XiangShan have been validated through mass production and adopted by multiple companies, while an ecosystem of tools and infrastructure now supports functional verification and performance exploration.</p>
    <p>The central challenge is soundness: agile verification must match the rigor of traditional methods while reducing human effort and verification time. LLMs and agents may further revolutionize chip design and verification, potentially enabling workflows with little or no human intervention.</p>
    <p>ADVC invites experts from academia and industry to share experience and vision, welcoming traditional approaches such as formal verification and fuzzing alongside emerging AI-driven methods.</p>
  </div>
</section>

<section class="section history">
  <div class="section-heading">
    <p class="section-kicker">02 / Community</p>
    <h2>A growing practice<br>behind the workshop.</h2>
  </div>
  <div class="reading-width lead-copy">
    <p class="lede">A new workshop, grounded in an active community.</p>
    <p>This particular workshop has not been held before. The organizers have previously led multiple XiangShan tutorials:</p>
    <ul>
      {% for workshop_event in workshop.previous_workshops %}
        <li>{{ workshop_event }}</li>
      {% endfor %}
    </ul>
    <p>Expected attendance: {{ workshop.expected_attendance }}. The workshop welcomes participants from both academia and industry.</p>
  </div>
</section>

<section class="section topics">
  <div class="section-heading">
    <p class="section-kicker">03 / Topics</p>
    <h2>Methods for building<br>and proving better chips.</h2>
  </div>
  <div class="topic-list">
    {% for topic in workshop.topics %}
      <article>
        <span class="topic-number">0{{ forloop.index }}</span>
        <h3>{{ topic.title }}</h3>
        <p>{{ topic.description }}</p>
      </article>
    {% endfor %}
  </div>
</section>

<section class="section invitation">
  <p class="section-kicker">Join the conversation</p>
  <div>
    <h2>Bring your paper,<br>experience, and perspective.</h2>
    <p>We welcome papers and presentations from academia and industry, including formal verification, fuzzing, and emerging AI-driven approaches.</p>
    <a class="button button-dark" href="{{ '/cfp/' | relative_url }}">Read the Call for Papers <span aria-hidden="true">→</span></a>
  </div>
</section>
