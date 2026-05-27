---
layout: home
author_profile: true
---
<div class="intro-text">
 Welcome! I am Oladayo, a Data Engineer focused on architecting efficient data pipelines and clean data models. I specialize in Python, SQL, and cloud infrastructure, ensuring data is accurate, accessible, and ready for analytics. Whether I am building end-to-end data pipelines or instructing college students in foundational computer science, I care deeply about writing clean code and building solid architecture. <br> <br> I am currently looking for my next engineering role within a corporate or academic institution. Take a look at my featured projects below
</div>

<h2>Projects</h2>
<div class="projects-grid">
  {% for post in site.posts %}
    <div class="project-card">
      <h3>{{ post.title }}</h3>
      <div class="project-content">
        {{ post.content }}
      </div>
      <div class="project-tools">
        <h4>Tools Used:</h4>
        <ul>
          {% for tool in post.tools %}
            <li><i class="{{ tool.icon }}"></i> {{ tool.name }}</li>
          {% endfor %}
        </ul>
      </div>
      <div class="project-links">
        {% for link in post.links %}
          <a href="{{ link.url }}" class="arrow-link" target="_blank" rel="noopener noreferrer">
            {{ link.title }} &#8594;
          </a>
        {% endfor %}
      </div>
    </div>
  {% endfor %}
</div>
