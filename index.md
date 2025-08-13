---
layout: home
author_profile: true
---
<div class="intro-text">
 Welcome to my portfolio! I am Oladayo, a data engineer passionate about building and maintaining data pipelines. I recently graduated from the University of Nottingham with a Master's degree. <br> <br> As I navigate the current job market, I am dedicated to continuously developing my skills in areas like Python, SQL, and cloud technologies through projects and sharing my learnings here. Explore my projects below to see my work.
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