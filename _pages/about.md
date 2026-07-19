---
permalink: /
title: ""
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<!-- <style>
  /* --- Layout & Width Architecture --- */
  @media (min-width: 64em) {
    #main {
      max-width: 1200px !important;
      display: flex !important;
      justify-content: space-between !important;
    }
    .page {
      flex-grow: 1 !important;
      max-width: calc(100% - 260px) !important;
      padding-left: 40px !important;
      padding-right: 0 !important;
    }
    .page__content {
      width: 100% !important;
      max-width: 100% !important;
    }
  }

  /* --- Premium Typography & Canvas Colors --- */
  body {
    background-color: #ffffff !important;
  }
  .page__content, p, li, dt, dd {
    color: #1e293b !important;
  }
  h1, h2, h3, h4, h5, h6 {
    color: #0f172a !important;
  }

  /* --- Interactive Anchors --- */
  a {
    color: #0256cc !important;
    text-decoration: none !important;
  }
  a:hover {
    color: #0284c7 !important;
    text-decoration: underline !important;
  }

  /* --- Premium Masthead Navigation Pills --- */
  .greedy-nav a,
  .greedy-nav a:hover,
  .greedy-nav a:focus,
  .visible-links a,
  .visible-links a:hover {
    text-decoration: none !important;
    border-bottom: none !important;
    box-shadow: none !important;
  }

  .greedy-nav .visible-links a {
    padding: 0.5em 0.8em !important;
    border-radius: 6px !important;
    transition: background-color 0.2s ease, color 0.2s ease !important;
  }

  .greedy-nav .visible-links a:hover {
    background-color: #f1f5f9 !important;
    color: #0f172a !important;
    text-decoration: none !important;
  }

  /* --- Clean Announcement Box --- */
  blockquote {
    background: #f8fafc !important;
    border-left: 4px solid #0f172a !important;
    padding: 1.2em 1.5em !important;
    font-style: normal !important;
    border-radius: 0 8px 8px 0;
    margin: 1.5em 0 !important;
    box-shadow: 0 1px 3px rgba(0,0,0,0.05) !important;
  }
  blockquote p {
    color: #334155 !important;
    margin: 0 !important;
    font-weight: 500 !important;

  /* --- Active/Current Tab Highlight --- */
  .greedy-nav .visible-links a.active,
  .greedy-nav .visible-links a[aria-current="page"],
  .greedy-nav .visible-links .current a,
  .greedy-nav .visible-links .current_page_item a {
    background-color: #0f172a !important; /* Premium dark slate background for the active page */
    color: #ffffff !important;            /* High contrast white text for maximum visibility */
    font-weight: 600 !important;
    text-decoration: none !important;
  }
</style> -->

<h1 style="font-size: 2.8em; margin-top: 0; margin-bottom: 0.2em; font-weight: 800; letter-spacing: -0.03em;">Hi!</h1>

> 🔍 **Looking for Opportunities:** I am actively seeking microarchitecture, systems, and security internship roles for Summer 2027.

I am a Computer Science Ph.D. student at Purdue University, advised by Dr. Kazem Taram in the SecArch Lab. My research focuses on **hardware security** and **microarchitecture**, with specific expertise in identifying **microarchitectural vulnerabilities**, conducting **side-channel analysis**, and engineering **protocol-level mitigations** for **Compute Express Link (CXL)** architectures and disaggregated memory systems. I am open to industry R&D collaborations, technical discussions, and advanced systems engineering opportunities.

<hr>
## 📰 Latest News

<!-- Added max-height, overflow-y, and a bit of right padding so text doesn't hug the scrollbar -->
<div style="margin-top: 1.5em; max-height: 300px; overflow-y: auto; padding-right: 10px;">
  {% for item in site.data.news %}
    <div style="display: flex; margin-bottom: 1em; align-items: flex-start;">
      <div style="min-width: 90px; font-weight: bold; color: #5b616a; flex-shrink: 0;">{{ item.date }}</div>
      <div style="flex-grow: 1; padding-left: 10px;">{{ item.text | markdownify | remove: '<p>' | remove: '</p>' }}</div>
    </div>
  {% endfor %}
</div>