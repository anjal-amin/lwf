---
layout: default
---

<div class="home">

  <!-- Add the logo image here -->
  <img src="{{ 'assets/images/lw-logo.png' | relative_url }}" alt="Logo" class="logo">
  <p>{{ site.description }}</p>

  {% assign latest_post = site.posts | first %}
  <article>
    <h2>{{ latest_post.title }}</h2>
    <div class="post-content">
      {{ latest_post.content }}
    </div>
  </article>
</div>

