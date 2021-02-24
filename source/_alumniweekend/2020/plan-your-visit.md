---
title: Plan your visit
description: 'Plan your Alumni Weekend 2020 with hotel deals and discounts, parking information, interactive map, and directions'
layout: page
category: aw-2020
order: 5

plan:
  - headline: Places to stay
    description: Several local hotels have set aside rooms for Alumni Weekend guests, with some offering special rates.
    image: /assets/images/hotels.jpg
    link: /alumniweekend/2020/hotels
  - headline: Parking information
    description: All you need to know about parking on campus for Alumni Weekend. Check back often for updated information as the weekend draws closer.
    image: /assets/images/parking.jpg
    link: /alumniweekend/2020/parking
  - headline: Campus interactive map
    description: This interactive map will help you find your way around campus.
    image: /assets/images/interactive-map.jpg
    link: https://www.ucsc.edu/map/
  - headline: Directions to campus
    description: Hop in the car—several major highways run to Santa Cruz. Or come by plane—the San Francisco and San Jose international airports, as well as Monterey Regional Airport, are all nearby.
    image: /assets/images/ucsc-map-300x252.gif
    link: /alumniweekend/2020/directions

nav: yes

published: true
    
---
{: .underline}
## {{ page.title }}

{% if page.plan %}
<div class="generic-card-list fade-out-siblings">
   {% for plan in page.plan %}
    <a class="generic-card" href="{{ plan.link }}" aria-label="">
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
