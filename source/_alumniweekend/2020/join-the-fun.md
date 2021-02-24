---
title: Join the fun
description: "Join the fun at Alumni Weekend: Be a volunteer or be a sponsor"
layout: page
category: aw-2020
order: 4
plan:
  - headline: Be a volunteer
    description: Join us for Alumni Weekend 2018! Friday, April 27–Sunday, April 29. With so many fun events happening, we don’t want any Slugs to miss out!
    image: /assets/images/2020/be-volunteer-2019.jpg
    link: /alumniweekend/2020/volunteer.html
  - headline: Sponsorship information
    description: Alumni Weekend presents a great opportunity for businesses to be seen as a partner of the university and its broad alumni population.
    image: /assets/images/2020/signatures.jpg
    link: /alumniweekend/2020/parking.html

published: true
---
{: .underline}
## {{ page.title }}

{% if page.plan %}
<div class="generic-card-list fade-out-siblings ">
   {% for plan in page.plan %}
    <a class="generic-card large-12" href="{{ plan.link }}" aria-label="">
        <div class="image">
            <img src="{{ plan.image }}">
        </div>
        <div class="card-text">
            <h4 class="underline">{{ plan.headline }}</h4>
            <p>{{ plan.description }}</p>
        </div>
    </a>
    {% endfor %}
</div>
{% endif %}
