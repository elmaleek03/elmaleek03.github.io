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
        <div class="fetch__group">Hello</div>

        <div class="fetch__row"><span class="fetch__icon">▸</span><span class="fetch__key">Name:</span><span class="fetch__val fetch__val--accent">Fajar Iman</span></div>
        <div class="fetch__row"><span class="fetch__icon">▸</span><span class="fetch__key">About:</span><span class="fetch__val">I like building things, solving problems, and learning as I go. Mostly mobile apps, backend services, and IT/networking.</span></div>

        <hr class="fetch__sep" />

        <div class="fetch__row"><span class="fetch__icon">▸</span><span class="fetch__key">Stack:</span><span class="fetch__val fetch__val--accent">Flutter · Go · C# · Firebase · Networking</span></div>
        <div class="fetch__row"><span class="fetch__icon">▸</span><span class="fetch__key">Focus:</span><span class="fetch__val">Mobile apps · Backend services · IT / Networking</span></div>

        <hr class="fetch__sep" />

        <div class="fetch__row"><span class="fetch__icon">▸</span><span class="fetch__key">Location:</span><span class="fetch__val">Depok, Indonesia</span></div>
      </div>

      <div class="fetch__footer">
        <a class="btn btn--primary" href="/about/">more about me →</a>
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
