---
layout: default
---

<div class="home">
  <h1>{{ site.title }}</h1>
  <p>{{ site.description }}</p>

  {% assign latest_post = site.posts | first %}
  <article>
    <h2>{{ latest_post.title }}</h2>
    <div class="post-content">
      {{ latest_post.content }}
    </div>
  </article>
</div>

