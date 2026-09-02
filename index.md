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
    <p>AI applications, particularly large language models and AI agents, are creating increasingly complex, diverse, and rapidly evolving computing demands. Specialized chips are becoming increasingly important, yet the high costs of conventional design tools, engineering effort, and IP, combined with long design cycles, make it difficult to keep pace with these changing demands.</p>
    <p>The hardware community is responding by embracing agile development and verification methodologies. Open, community-driven projects such as XiangShan have demonstrated the potential of this approach through production silicon and adoption by multiple companies. Meanwhile, a growing ecosystem of tools and infrastructure is enabling efficient functional verification and rapid performance exploration.</p>
    <p>The central challenge is soundness: agile verification must match the rigor of traditional methods while reducing human effort and verification time. LLMs and agents may further revolutionize chip design and verification, potentially enabling workflows with little or no human intervention.</p>
    <p>ADVC invites experts from academia and industry to share experience and vision, welcoming traditional approaches such as formal verification and fuzzing alongside emerging AI-driven methods.</p>
  </div>
</section>

<section class="section submission" id="cfp">
  <div class="content-grid">
    <div>
      <h2>Call for Papers</h2>
    </div>
    <div class="cfp-content">
      <section class="cfp-subsection" aria-labelledby="topics-of-interest">
        <h3 id="topics-of-interest">Topics of Interest</h3>
        <p>We invite papers on agile development and verification for chips. Submissions may present mature research, work in progress, industrial experience, or new directions for the community.</p>
        <ul>
          <li>Agile chip development and verification methods, including reusable tools, infrastructure, and experience from practice</li>
          <li>Rapid design-space exploration and rigorous verification, including
            <ul>
              <li>Agile microarchitectural exploration and PPA optimization</li>
              <li>Rapid compiler-hardware co-design and optimization</li>
              <li>Automated architectural security analysis and verification</li>
              <li>Scalable and efficient verification methodologies</li>
            </ul>
          </li>
          <li>Agile hardware development tools, infrastructure, or workflows for
            <ul>
              <li>Functional and performance verification</li>
              <li>Rapid performance exploration and evaluation</li>
              <li>Adoption of AI and AI agents in hardware development</li>
              <li>Acceleration of RTL simulation</li>
              <li>AI-native hardware programming languages</li>
            </ul>
          </li>
        </ul>
      </section>

      <section class="cfp-subsection" aria-labelledby="paper-submission">
        <h3 id="paper-submission">Paper Submission</h3>
        <p>Submissions may present a research result, a position or systems paper, an industrial experience report, or a demonstration of a verification tool, infrastructure, or open-source project.</p>
        <p>We welcome the following forms of contribution:</p>
        <ul>
          <li><strong>Research papers:</strong> completed research with a clear problem, method, experimental evaluation, and conclusions.</li>
          <li><strong>Position papers:</strong> perspectives on agile development or verification, including challenges, roadmaps, and open questions.</li>
          <li><strong>Systems papers:</strong> working toolchains, platforms, infrastructure, or end-to-end systems, supported by evidence from use or evaluation.</li>
          <li><strong>Industrial experience reports:</strong> workflows, scale, metrics, lessons learned, failures, and transferable insights from real projects.</li>
          <li><strong>Demonstrations:</strong> live presentations of tools, infrastructure, or open-source projects, describing the demonstration, its dependencies, and availability.</li>
        </ul>
        <a class="button" href="{{ workshop.submission_link }}">Submit</a>
      </section>
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
