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

<section class="section about">
  <div class="section-heading">
    <p class="section-kicker">01</p>
    <h2>Overview</h2>
  </div>
  <div class="reading-width lead-copy">
    <p class="lede">Agile development and verification for the next generation of chips.</p>
    <p>AI workloads are driving rapidly changing demand for customized chips, while traditional design methods remain costly and slow. ADVC 2026 brings together academia and industry to advance agile chip development and rigorous, efficient verification, spanning formal methods and fuzzing to emerging LLM- and agent-driven approaches.</p>
    <p>We welcome mature research, work in progress, industrial experience, and new directions that can help make chip development faster, more accessible, and dependable.</p>
  </div>
</section>

<section class="section dates">
  <div class="content-grid">
    <div>
      <p class="section-kicker">02</p>
      <h2>Important Dates</h2>
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
      <p class="section-kicker">03</p>
      <h2>Topics of Interest</h2>
    </div>
    <div>
      <p>We invite papers on agile development and verification for chips. Submissions may present mature research, work in progress, industrial experience, or new directions for the community.</p>
      <ul>
        <li>Research based on or evaluated using XiangShan, XS-GEM5, or XSAI</li>
        <li>Optimizations for XiangShan, including
          <ul>
            <li>Microarchitectural features for improved PPA (power, performance, and area)</li>
            <li>Compiler optimizations targeting the XiangShan microarchitecture</li>
            <li>Architectural security of XiangShan</li>
            <li>Testing and verification of XiangShan</li>
            <li>Calibration between XiangShan and XS-GEM5</li>
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
    </div>
  </div>
</section>

<section class="section">
  <div class="content-grid">
    <div>
      <p class="section-kicker">04</p>
      <h2>Paper Submission</h2>
    </div>
    <div>
      <p>Submissions may present a research result, a position or systems paper, an industrial experience report, or a demonstration of a verification tool, infrastructure, or open-source project.</p>
      <ul>
        {% for type in workshop.contribution_types %}
          <li>{{ type }}</li>
        {% endfor %}
      </ul>
      <p>We welcome the following forms of contribution:</p>
      <ul>
        <li><strong>Research papers:</strong> completed research with a clear problem, method, experimental evaluation, and conclusions.</li>
        <li><strong>Position papers:</strong> perspectives on agile development or verification, including challenges, roadmaps, and open questions.</li>
        <li><strong>Systems papers:</strong> working toolchains, platforms, infrastructure, or end-to-end systems, supported by evidence from use or evaluation.</li>
        <li><strong>Industrial experience reports:</strong> workflows, scale, metrics, lessons learned, failures, and transferable insights from real projects.</li>
        <li><strong>Demonstrations:</strong> live presentations of tools, infrastructure, or open-source projects, describing the demonstration, its dependencies, and availability.</li>
      </ul>
      <p class="notice">Submission portal, paper length, and formatting requirements will be announced when the call opens.</p>
      <a class="button button-dark" href="mailto:{{ workshop.contact_email }}?subject=ADVC%202026%20paper">Contact the organizers</a>
    </div>
  </div>
</section>
