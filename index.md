---
layout: default
title: "Mohan Elapolu"
nav_exclude: true
---

<style>
  body {
    scroll-behavior: smooth;
  }
  section {
    padding: 40px 0;
    border-bottom: 1px solid #ddd;
  }
  h2 {
    margin-top: 40px;
  }
</style>

<nav class="site-nav" style="margin-bottom: 40px;">
  <a href="#home">Home</a> |
  <a href="#about">About</a> |
  <a href="#research">Research</a> |
  <a href="#projects">Projects</a>
</nav>

<!-- HOME SECTION -->
<section id="home">
  <h2>Latest Posts</h2>

  {% for post in site.posts limit:3 %}
  <div style="margin-bottom:20px;">
    <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
    <small>{{ post.date | date: "%B %d, %Y" }}</small>
    <p>{{ post.excerpt }}</p>
  </div>
  {% endfor %}

  <p><a href="/posts/">View all posts →</a></p>
</section>

<!-- ABOUT SECTION -->
<section id="about">
  <h2>About Me</h2>

  {% markdown %}
  Hi, I'm **Mohan Elapolu**.

  - AI / ML  
  - Research  
  - Writing

  I enjoy learning, building, and publishing my thoughts online.
  {% endmarkdown %}
</section>

<!-- RESEARCH SECTION -->
<section id="research">
  <h2>Research</h2>
  {% markdown %}
  - **Topic 1** — short description  
  - **Topic 2** — short description  
  - **Topic 3** — short description  

  Add your actual research summaries here.
  {% endmarkdown %}
</section>

<!-- PROJECTS SECTION -->
<section id="projects">
  <h2>Projects</h2>
  {% markdown %}
  - **Project 1** — description — [GitHub link](#)  
  - **Project 2** — description — [GitHub link](#)  
  - **Project 3** — description — [GitHub link](#)  
  {% endmarkdown %}
</section>