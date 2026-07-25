---
layout: home
author_profile: true
---
<div class="intro-text">
  I am Oladayo, a Data Engineer specializing in <strong>data pipeline engineering</strong> and <strong>analytical data modeling</strong> (relational 3NF & Kimball star schemas). I build maintainable, cloud-native data architectures using Python, SQL, dbt, Terraform, Docker, and GCP to deliver reliable, analytics-ready datasets. I also instruct university-bound students in computer science fundamentals.
</div>

<div class="category-block" id="data-pipeline-engineering">
  <h2 class="category-heading"><i class="fas fa-network-wired"></i> Data Pipeline Engineering</h2>
  <div class="projects-grid">
    {% assign pipeline_posts = site.posts | where: "category", "data-pipeline-engineering" %}
    {% for post in pipeline_posts %}
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
</div>

<div class="category-block" id="analytical-pipeline-engineering">
  <h2 class="category-heading"><i class="fas fa-cubes"></i> Analytical Pipeline Engineering (Data Modelling)</h2>
  <div class="projects-grid">
    {% assign modelling_posts = site.posts | where: "category", "analytical-pipeline-engineering" %}
    {% for post in modelling_posts %}
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
</div>
