---
layout: front-page
title: Alumni Weekend
description: UC Santa Cruz Alumni Weekend 2020, April 3-5.
category: aw-2020
billboard:
  subtitle: Reconnect, reignite, remember
  image: /assets/images/billboard/2020/homepage-billboard.jpg
  image-2: /assets/images/billboard/2020/homepage-billboard-v2.jpg
  alt-text: "Friday-Sunday, Alumni Weekend April 3-5, 2020"
  hero-title: Alumni Weekend
  day: Friday–Sunday
  month: April
  date: 3–5
  year: 2020
  register-url: '#'

published: true
---

<section class="content-w-media left haltered blue">
  <div class="grid-container large">
    <div class="inner">
      <div class="content">
          <h2 class="underline"><a href="/atwood">Margaret Atwood at UC Santa Cruz</a></h2>
          <h5 style="font-weight: 500">Date: April 5, 2020</h5>
          <p>Join us as we welcome award-winning author Margaret Atwood—whose books include <em>The Handmaid's Tale</em> and its brand-new sequel, <em>The Testaments</em>—to campus on Sunday, April 5, for an onstage discussion with alumna and bestselling author Kate Schatz as part of the Baskin Ethics Lecture series.</p>
          <div class="content-foot-links">
            <a class="btn-link" href="/atwood">Event Info</a>
            <a class="button primary expanded" href="https://ucsctickets.universitytickets.com/w/event.aspx?id=1467">Buy Tickets</a>
          </div>
      </div>
      <div class="media">
          <img src="/atwood/images/atwood-homepage.jpg" alt="Margaret Atwood">
      </div>
    </div>
  </div>
</section>


<section class="heading">
  <h2 class="underline">Thank you to our sponsors</h2>
</section>

{% if site.data.sponsors-2020.platinum != null %}
<section class="heading">
    <h3>Platinum Sponsors</h3>
</section>
<div class="grid-container large mt-25">
  <div class="grid-x grid-margin-x align-center">
    {% for platinum in site.data.sponsors-2020.platinum %}
      <div class="cell large-6">
        <div class="closing-blocks">
          <a href="{{ platinum.url }}">
            <div class="image">
              <img src="{{ platinum.img }}" alt="{{ platinum.alt }}">
            </div>
          </a>
        </div>
      </div>
    {% endfor %}
  </div>
</div>
{% endif %}


{% if site.data.sponsors-2020.gold != null %}
<section class="heading">
    <h3>Gold Sponsor</h3>
</section>

<div class="grid-container large mt-25">
  <div class="grid-x grid-margin-x align-center">
    {% for gold in site.data.sponsors-2020.gold %}
      <div class="cell large-5">
        <div class="closing-blocks">
          <a href="{{ gold.url }}">
            <div class="image">
              <img src="{{ gold.img }}" alt="{{ gold.alt }}">
            </div>
          </a>
        </div>
      </div>
    {% endfor %}
  </div>
</div>
{% endif %}

{% if site.data.sponsors-2020.bronze != null %}
<section class="heading">
    <h3>Bronze Sponsor</h3>
</section>

<div class="grid-container large mt-25">
  <div class="grid-x grid-margin-x align-center">
   {% for bronze in site.data.sponsors-2020.bronze %}
      <div class="cell large-4">
        <div class="closing-blocks">
          <a href="{{ bronze.url }}">
            <div class="image">
              <img src="{{ bronze.img }}" alt="{{ bronze.alt }}">
            </div>
          </a>
        </div>
      </div>
    {% endfor %}
  </div>
</div>
<p></p>
{% endif %}


{% if site.data.sponsors-2020.inkind != null %}
<section class="heading">
    <h3>In-kind Sponsors</h3>
</section>

<div class="grid-container large mt-25">
  <div class="grid-x grid-margin-x align-center">
    {% for inkind in site.data.sponsors-2020.inkind %}
      <div class="cell small-6 large-3 xlarge-2">
        <div class="closing-blocks">
          <a href="{{ inkind.url }}">
            <div class="image">
              <img src="{{ inkind.img }}" alt="{{ inkind.alt }}">
            </div>
          </a>
        </div>
      </div>
    {% endfor %}
  </div>
</div>
<p></p>
{% endif %}

