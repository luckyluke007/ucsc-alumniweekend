---
layout: front-page
title: Alumni Reunion Weekend
description: "Alumni Reunion Weekend will celebrate our Golden Slug alumni from the classes of 1965-1973."

category: "aw-2024"
order: 1
og-image: "https://alumniweekend.ucsc.edu/assets/images/2024/banner.png"

---



<style>
  .page-utilities {
    display: none;
  }
</style>


{% for information in page.information %}
<section class="content-w-media {{ information.layout }}" style="margin: 0">
  <div class="grid-container large">
    <div class="inner">
      <div class="content">
        <h2 class="underline">{{ information.title }}</h2>
        <p>{{ information.description }}</p>
      </div>
      <div class="media">
          <img src="{{ information.image }}">
      </div>
    </div>
  </div>
</section>
{% endfor %}