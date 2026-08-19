---
layout: default
title: Call for Papers
description: Submission information and important dates for ADVC 2026.
---

{% assign workshop = site.data.workshop %}

<section class="page-heading" id="top">
  <p class="eyebrow">01 / Participate</p>
  <h1>Call for Papers</h1>
  <p>{{ workshop.title }}</p>
</section>

<section class="section dates">
  <div class="content-grid">
    <div>
      <p class="section-kicker">Important dates</p>
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
