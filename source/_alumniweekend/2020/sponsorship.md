---
title: Be a sponsor
description: 'Alumni Weekend presents a great opportunity for businesses to be seen as a partner of the university and its broad alumni population.'
layout: page
category: aw-2020
order: 4
nav: yes
---

## How to be an Alumni Weekend sponsor

**[Register to be a sponsor](https://secure.ucsc.edu/s/1069/bp18/interior.aspx?sid=1069&gid=1001&pgid=3959&cid=7946)**


### Why get involved?

Alumni Weekend presents a great opportunity for businesses to be seen as a partner of the university and its broad alumni population. With more than 1,000 attendees and 60-plus events throughout the three-day celebration, Alumni Weekend is a perfect time to be part of the occasion with the campus and the community. 

### Marketing benefits

Alumni Weekend successfully draws alumni back to campus through marketing promotion and cobranding opportunities in print, radio, mailing, and email (which reaches our 110,000-plus alumni base). Many of our past alumni attendees have stated in surveys that their preferred way to engage with the campus is through Alumni Weekend. 

### Join us!

In short, Alumni Weekend continues to be a key moment to celebrate our alumni. It is the one time of year the Banana Slug family and the community come together to enjoy a unique, festive, and stimulating experience. With increasing attendance, continued support, and wonderful collaboration between the campus and Santa Cruz communities, we invite you to be our partner and celebrate with us all weekend long!


Contact:

**Alexandra Sibille**<br/>
Assistant director of business development<br/>
**Email:** [asibille@ucsc.edu](mailto:asibille@ucsc.edu)<br/>
**Phone:** (831) 332-6620<br/>

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
      <div class="cell large-5">
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
      <div class="cell large-4">
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
      <div class="cell large-3">
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
      <div class="cell large-2">
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
