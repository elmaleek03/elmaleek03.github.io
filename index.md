---
layout: home
title: Home
---

<!-- Hero -->
<section class="hero">
  <h1 class="hero__title">Hi, I’m <span class="accent">Your Name</span>.</h1>
  <p class="hero__subtitle">
    Mobile app developer (Flutter). I build practical tools, experiment with backend/infra,
    and write my thoughts here.
  </p>

  <div class="hero__cta">
    <a class="btn btn--primary" href="/blog/">Read the blog</a>
    <a class="btn btn--ghost" href="/about/">About me</a>
  </div>

  <div class="hero__meta">
    <span>📍 Indonesia</span>
    <span>🧰 Flutter • Firebase • Go • AWS</span>
  </div>
</section>

<hr class="sep" />

<!-- Featured / Latest posts -->
<section>
  <div class="section__head">
    <h2>Latest writing</h2>
    <a class="muted" href="/blog/">View all →</a>
  </div>

  <div class="postlist">
    {% for post in site.posts limit: 5 %}
      <a class="postcard" href="{{ post.url }}">
        <div class="postcard__top">
          <h3 class="postcard__title">{{ post.title }}</h3>
          <time class="postcard__date" datetime="{{ post.date | date_to_xmlschema }}">
            {{ post.date | date: "%d %b %Y" }}
          </time>
        </div>

        {% if post.excerpt %}
          <p class="postcard__excerpt">{{ post.excerpt | strip_html | truncate: 160 }}</p>
        {% endif %}

        <div class="postcard__tags">
          {% if post.tags %}
            {% for tag in post.tags limit: 3 %}
              <span class="tag">{{ tag }}</span>
            {% endfor %}
          {% endif %}
        </div>
      </a>
    {% endfor %}
  </div>
</section>
