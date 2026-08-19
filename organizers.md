---
layout: default
title: Organizers
description: Organizing team for ADVC 2026.
---

{% assign workshop = site.data.workshop %}

<section class="page-heading" id="top">
  <p class="eyebrow">03 / People</p>
  <h1>Organizers</h1>
  <p>{{ workshop.title }}</p>
</section>

<section class="section organizers">
  <p class="section-kicker">Organization</p>
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
