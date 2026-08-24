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

<section class="section topics" id="topics">
  <div class="section-heading">
    <p class="section-kicker">02 / Topics</p>
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
    <a class="button button-dark" href="#cfp">Read the Call for Papers <span aria-hidden="true">↓</span></a>
  </div>
</section>

<section class="section dates" id="cfp">
  <div class="content-grid">
    <div>
      <p class="section-kicker">03 / Participate</p>
      <h2>Key dates</h2>
    </div>
    <div class="dates-table">
      <div><span>Submission deadline</span><strong>To be announced</strong></div>
      <div><span>Notification</span><strong>To be announced</strong></div>
      <div><span>Workshop</span><strong>{{ workshop.date }} · {{ workshop.duration }}</strong></div>
    </div>
  </div>
</section>

<section class="section submission">
  <div class="content-grid">
    <div>
      <p class="section-kicker">Paper submission</p>
      <h2>How to submit</h2>
    </div>
    <div>
      <p>We invite papers on agile development and verification for chips. Submissions may present mature research, work in progress, industrial experience, or new directions for the community.</p>
      <ul>
        {% for type in workshop.contribution_types %}
          <li>{{ type }}</li>
        {% endfor %}
      </ul>
      <p class="notice">Submission portal, paper length, and formatting requirements will be announced when the call opens.</p>
      <a class="button" href="mailto:{{ workshop.contact_email }}?subject=ADVC%202026%20paper">Contact the organizers</a>
    </div>
  </div>
</section>

<section class="section program" id="program">
  <p class="section-kicker">04 / Attend</p>
  <h2>Program</h2>
  <p class="program-lead">The detailed agenda and invited speakers will be announced closer to the workshop. Invited talks are currently TBD.</p>
  <div class="program-table">
    <div><strong>Opening remarks</strong><span>Workshop overview and community discussion</span></div>
    <div><strong>Invited talks</strong><span>Perspectives from academia and industry (TBD)</span></div>
    <div><strong>Paper presentations</strong><span>Peer-reviewed work on agile chip development and verification</span></div>
    <div><strong>Discussion</strong><span>Challenges and opportunities for reliable, efficient chip verification</span></div>
  </div>
</section>

<section class="section organizers" id="organizers">
  <p class="section-kicker">05 / People</p>
  <h2>Organizing Team</h2>
  <div class="organizer-list">
    {% for organizer in workshop.organizers %}
      <article>
        <h3>{{ organizer.name }}</h3>
        <p>{{ organizer.affiliation }}</p>
      </article>
    {% endfor %}
  </div>
</section>

<section class="section inclusion">
  <div class="content-grid">
    <div>
      <p class="section-kicker">Diversity and inclusion</p>
      <h2>Many disciplines,<br>one conversation.</h2>
    </div>
    <div>
      <p>ADVC welcomes participation from both academia and industry. Invited speakers will include experts from both communities, with attention to diversity in gender and racial backgrounds.</p>
    </div>
  </div>
</section>

<section class="section invited">
  <div class="content-grid">
    <div>
      <p class="section-kicker">Invited talks</p>
      <h2>Perspectives from<br>the field.</h2>
    </div>
    <div>
      <p>Invited speakers will be announced in the program. Current status: TBD.</p>
    </div>
  </div>
</section>
