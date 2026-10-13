---
layout: home
title: Home
---

<!-- Hero: fastfetch-style fetch output -->
<section class="hero">
  <p class="hero__line"><span class="prompt">visitor@elmaleeks-website:~$</span> fetch<span class="cursor"></span></p>

  <div class="fetch">
    <div class="fetch__art">
      {% include ascii-face.html %}
    </div>

    <div class="fetch__info">
      <div class="fetch__box">
        <div class="fetch__group">Hello World</div>

        <div class="fetch__output">
          <p>I'm Fajar Iman, a tech enthusiast who enjoys discovering new things, solving problems, and building solutions. Currently most of my days go into mobile apps, backend services, and IT/networking.</p>

          <p>I like figuring out how systems work, breaking them (sometimes), and making them better. This site is where I share what I'm learning, building, and experimenting with along the way. I hope i could share and write my journeys here lol.</p>

          <p class="fetch__output-note"><span class="fetch__caret">&gt;</span> Currently learning on CI/CD, Deployment, Ubuntu Servers, and AI Orchestration.</p>
        </div>

        <div class="fetch__footer">
          <a class="btn btn--primary" href="/about/">more about me →</a>
        </div>
      </div>
    </div>
  </div>
</section>

<hr class="sep" />

<!-- Latest posts -->
<section>
  <div class="section__head">
    <h2>latest writing</h2>
  </div>

  <div class="postlist">
    {% for post in site.posts limit: 5 %}
      <a class="postcard" href="{{ post.url }}">
        <div class="postcard__top">
          <h3 class="postcard__title">{{ post.title }}</h3>
          <time class="postcard__date" datetime="{{ post.date | date_to_xmlschema }}">
            {{ post.date | date: "%Y-%m-%d" }}
          </time>
        </div>

        {% if post.excerpt %}
          <p class="postcard__excerpt">{{ post.excerpt | strip_html | truncate: 140 }}</p>
        {% endif %}
      </a>
    {% endfor %}
  </div>

  <div class="section__foot">
    <a class="btn btn--primary" href="/blog/">see all writing →</a>
  </div>
</section>
