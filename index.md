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
        <a class="button button-accent" href="#cfp">View the call for papers <span aria-hidden="true">↓</span></a>
        <a class="text-link" href="#about">Explore the workshop <span aria-hidden="true">↓</span></a>
      </div>
    </div>
  </div>
  <dl class="event-strip" aria-label="Workshop information">
    <div><dt>Date</dt><dd>{{ workshop.date }}</dd></div>
    <div><dt>Location</dt><dd>{{ workshop.location }}</dd></div>
    <div><dt>Presented at</dt><dd><a href="{{ workshop.micro_workshops_url }}" target="_blank" rel="noreferrer">{{ workshop.conference }} <span aria-hidden="true">↗</span></a></dd></div>
  </dl>
</section>

<section class="section about" id="about">
  <div class="section-heading">
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

<section class="section submission" id="cfp">
  <div class="content-grid">
    <div>
      <h2>Call for Papers</h2>
    </div>
    <div>
      <p>We invite papers on agile development and verification for chips. Submissions may present mature research, work in progress, industrial experience, or new directions for the community.</p>
      <ul>
        {% for type in workshop.contribution_types %}
          <li>{{ type }}</li>
        {% endfor %}
      </ul>
      <p class="notice">Submission portal, paper length, and formatting requirements will be announced when the call opens.</p>
      <a class="button" href="{{ workshop.submission_link }}">Submit</a>
    </div>
  </div>
</section>

<section class="section dates">
  <div class="content-grid">
    <div>
      <h2>Important dates</h2>
    </div>
    <div class="dates-table">
      <div><span>Submission deadline</span><strong>{{ workshop.submission_deadline }}</strong></div>
      <div><span>Notification</span><strong>{{ workshop.notification_date }}</strong></div>
      <div><span>Workshop</span><strong>{{ workshop.date }} · {{ workshop.duration }}</strong></div>
    </div>
  </div>
</section>

{% if workshop.show_program %}
  <section class="section program" id="program">
    <h2>Program</h2>
    <div class="program-table">
      <div><strong>Opening remarks</strong><span>Workshop overview and community discussion</span></div>
      <div><strong>Invited talks</strong><span>Perspectives from academia and industry (TBD)</span></div>
      <div><strong>Paper presentations</strong><span>Peer-reviewed work on agile chip development and verification</span></div>
      <div><strong>Discussion</strong><span>Challenges and opportunities for reliable, efficient chip verification</span></div>
    </div>
  </section>
{% endif %}

<section class="section organizers" id="organizers">
  <h2>Organizers</h2>
  <div class="organizer-list">
    {% for organizer in workshop.organizers %}
      <article>
        <h3><a href="{{ organizer.homepage }}" target="_blank" rel="noreferrer">{{ organizer.name }}</a></h3>
        <p class="organizer-title">{{ organizer.title }}</p>
        <p>{{ organizer.affiliation }}</p>
      </article>
    {% endfor %}
  </div>
</section>
