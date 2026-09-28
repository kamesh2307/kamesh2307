---
layout: home
title: "Kamesh Murty — Strategy & Market Intelligence"
permalink: /
hero_image: /assets/images/hero.jpg
---

<style>
/* Minimal page styling — works with most Jekyll themes */
.container{max-width:1100px;margin:0 auto;padding:28px}
.grid{display:grid;grid-template-columns:320px 1fr;gap:28px;align-items:start}
.card{background:#fff;border-radius:12px;padding:20px;border:1px solid #eef2f7}
.avatar{width:96px;height:96px;border-radius:12px;background:linear-gradient(135deg,#0ea5a4,#6366f1);display:flex;align-items:center;justify-content:center;color:#fff;font-weight:700;font-size:28px}
.chips{display:flex;gap:8px;flex-wrap:wrap;margin-top:12px}
.chip{background:#f8fafb;padding:8px 10px;border-radius:999px;border:1px solid #eef6f5;font-size:13px}
.project{border-radius:10px;padding:14px;background:linear-gradient(180deg,#ffffff,#fbfdff);border:1px solid #eef2f7;margin-bottom:12px}
.meta{color:#556070;font-size:14px}
blockquote.profile{background:#fbfffe;border-left:4px solid #e6f6f5;padding:12px;border-radius:6px;color:#24303a}
@media (max-width:920px){.grid{grid-template-columns:1fr}}
</style>

<div class="container">
  <div class="grid">
    <!-- Sidebar -->
    <aside class="card" aria-label="Profile sidebar">
      <div class="avatar" aria-hidden="true">KM</div>
      <h2 style="margin:10px 0 4px 0">Kamesh Murty</h2>
      <div class="meta" style="margin-bottom:12px">Senior Industry Analyst — Strategy · Pune Division, Maharashtra, India</div>

      <h4 style="margin-top:8px">Contact</h4>
      <div class="meta"><strong>Email</strong> — <a href="mailto:kameshmurty23@gmail.com">kameshmurty23@gmail.com</a></div>
      <div class="meta"><strong>Phone</strong> — <a href="tel:+917397915827">+91 73979 15827</a></div>
      <div class="meta"><strong>LinkedIn</strong> — <a href="https://www.linkedin.com/in/kamesh-murty" target="_blank" rel="noopener">linkedin.com/in/kamesh-murty</a></div>
      <div class="meta"><strong>GitHub</strong> — <a href="https://github.com/kamesh2307" target="_blank" rel="noopener">github.com/kamesh2307</a></div>

      <h4 style="margin-top:14px">Top Skills</h4>
      <div>
        <span class="chip">Microsoft Excel</span>
        <span class="chip">Microsoft Office</span>
        <span class="chip">Microsoft Word</span>
        <span class="chip">Market Forecasting</span>
        <span class="chip">Competitive Analysis</span>
      </div>

      <h4 style="margin-top:14px">Languages</h4>
      <div class="meta">English — Full Professional</div>
      <div class="meta">Telugu — Native or Bilingual</div>
      <div class="meta">Hindi — Native or Bilingual</div>
      <div class="meta">French — Limited Working</div>

      <h4 style="margin-top:14px">Education</h4>
      <div class="meta"><strong>MBA</strong> — Symbiosis Institute of International Business (Energy & Environment), 2016–2018</div>
      <div class="meta"><strong>B.Tech</strong> — Vellore Institute of Technology (Civil Engineering), 2011–2015</div>
    </aside>

    <!-- Main -->
    <main class="card" aria-label="Main content">
      <header>
        <h1 style="margin:0 0 6px 0">Kamesh Murty</h1>
        <div class="meta">Industry Strategy Specialist at Hyster-Yale · Market forecasting · Competitive analysis · Salesforce CRM</div>
      </header>

      <blockquote class="profile" style="margin-top:12px">
"I serve as the Industry Strategy Specialist at Hyster Yale Group, executing strategic projects & business asks, and report development for EMEA, Americas, and Asia Pacific theatres."  
"Graduating from a Top Tier Management School, I am a result driven professional with over 5+ years of expertise in Business Strategy, Business Development, and market research across diverse industries."
      </blockquote>

      <p style="margin-top:12px">
        I am a result-driven professional with 5+ years of experience in business strategy, business development, and market research across diverse industries. I execute strategic projects and develop reports for EMEA, Americas, and Asia Pacific theatres. Experienced in Salesforce CRM, market data analysis and strategy, market forecasting, competitive analysis and benchmarking. Passionate about collaborating with stakeholders to create measurable value.
      </p>

      <div class="chips" aria-hidden="true">
        <span class="chip">Market Forecasting</span>
        <span class="chip">Competitive Benchmarking</span>
        <span class="chip">Salesforce CRM</span>
        <span class="chip">Data Analysis</span>
      </div>

      <section style="margin-top:18px">
        <h2 style="margin:0 0 8px 0">Projects</h2>
        <p class="meta" style="margin-top:6px">Projects are read automatically from <code>projects/*/README.md</code>. Add a folder per project with a README to include it here.</p>

        <!-- Liquid loop: list projects from projects/*/README.md -->
        {% for p in site.pages %}
          {% if p.path contains 'projects/' and p.path != 'projects/README.md' and p.path endswith 'README.md' %}
            {% assign parts = p.path | split: '/' %}
            {% assign slug = parts[1] %}
            <article class="project" id="{{ slug }}">
              <h3 style="margin:0 0 6px 0"><a href="/projects/{{ slug }}/" style="text-decoration:none;color:inherit">{{ slug | replace: '-', ' ' | capitalize }}</a></h3>
              <div class="meta">
                {% comment %} If you include a first line like "Role: ..." in the project README, it will appear in the excerpt. {% endcomment %}
                {{ p.content | markdownify | strip_html | truncate: 280 }}
              </div>
            </article>
          {% endif %}
        {% endfor %}

      </section>

      <section class="experience" style="margin-top:18px">
        <h2 style="margin:0 0 8px 0">Experience</h2>

        <div style="margin-bottom:10px">
          <h4 style="margin:0">Industry Strategy Specialist I — Hyster-Yale Materials Handling</h4>
          <div class="meta">April 2025 – Present · Pune, Maharashtra, India</div>
          <p style="margin-top:8px">Execute strategic projects and report development for EMEA, Americas, and Asia Pacific theatres; market data analysis and strategy.</p>
        </div>

        <div style="margin-bottom:10px">
          <h4 style="margin:0">Senior Industry Analyst — Hyster-Yale Materials Handling</h4>
          <div class="meta">June 2022 – April 2025 · Pune, Maharashtra, India</div>
          <p style="margin-top:8px">Market forecasting, competitive analysis and benchmarking; stakeholder collaboration to drive organizational change.</p>
        </div>

        <div style="margin-bottom:10px">
          <h4 style="margin:0">Research Analyst — Verify Markets</h4>
          <div class="meta">June 2019 – June 2022 · Pune, Maharashtra, India</div>
          <p style="margin-top:8px">Market research and report writing across multiple sectors; Salesforce CRM experience.</p>
        </div>

        <div style="margin-bottom:10px">
          <h4 style="margin:0">Management Trainee — Bajaj Allianz Life</h4>
          <div class="meta">June 2018 – June 2019 · Pune / Hyderabad Area, India</div>
          <p style="margin-top:8px">Rotational exposure to operations and client servicing.</p>
        </div>
      </section>

      <section class="education" style="margin-top:18px">
        <h2 style="margin:0 0 8px 0">Education</h2>
        <div style="display:grid;grid-template-columns:repeat(auto-fit,minmax(220px,1fr));gap:12px">
          <div style="background:#fff;padding:12px;border-radius:8px;border:1px solid #eef2f7">
            <strong>Symbiosis Institute of International Business</strong><br/>MBA — Energy and Environment · 2016–2018
          </div>
          <div style="background:#fff;padding:12px;border-radius:8px;border:1px solid #eef2f7">
            <strong>Vellore Institute of Technology</strong><br/>B.Tech — Civil Engineering · 2011–2015
          </div>
          <div style="background:#fff;padding:12px;border-radius:8px;border:1px solid #eef2f7">
            <strong>Center Point School</strong><br/>H.S.C · 1999–2009
          </div>
        </div>
      </section>

      <footer style="margin-top:18px">
        <div class="meta">Available for consulting · Open to strategic collaborations</div>
        <div style="margin-top:8px">
          <a href="https://www.linkedin.com/in/kamesh-murty" target="_blank" rel="noopener">LinkedIn</a> ·
          <a href="https://github.com/kamesh2307" target="_blank" rel="noopener">GitHub</a>
        </div>
      </footer>
    </main>
  </div>
</div>
