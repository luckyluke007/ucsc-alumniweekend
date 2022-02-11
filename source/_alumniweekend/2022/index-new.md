---
layout: front-page-2022
title: Alumni Week 2022
description: "Celebrating Alumni Week in true 2022 style. Have fun, remember your roots, reignite your passions, and connect like never before as our first virtual Alumni Week zooms you back to campus."

category: aw-2022

billboard:
  date: "April 19-22, 2022"
  hero-title: "Alumni Week 2022"
  subhead: "Celebrating Alumni Voices"
  description: "Virtual & In Person"
  action-text: Register Now
  register-url: '#'

featured:
  - title: "University Forum with Julia Calderone & Nicholas St. Fleur"
    date: "2022-04-19"
    starttime: "5:30pm"
    endtime: "7:00pm"
    image: "/assets/images/2021/terri-mccullough.jpg"
    description: "Details to come"
    url: "https://calendar.ucsc.edu/event/university_forum_featuring_julia_calderone_nicholas_st_fleur#.YfrQrS-cbOQ"
  - title: "University Forum with Arts Dean"
    date: "2022-04-20"
    starttime: "5:30pm"
    endtime: "7:00pm"
    image: "/assets/images/2021/va-banner.jpg"
    description: "Details to come"
    url: "https://calendar.ucsc.edu/event/university_forum_with_arts_dean_celine_parrenas_shimizu#.YfrRMS-cbOQ"
  - title: "Strange Weather Alumni Reception at the MAH"
    date: "2022-04-22"
    starttime: "6:00pm"
    endtime: "8:00pm"
    image: "/assets/images/2021/uf-banner.jpg"
    description: "Details to come"
    url: "https://calendar.ucsc.edu/event/strange_weather_alumni_reception_at_the_mah#.YfrRfS-cbOQ"
  - title: 'Confronting Climate Change Conference - Community Fair'
    date: "2022-04-23"
    starttime: "10:00am"
    endtime: "4:00pm"
    image: "/assets/images/2021/comedy-errors-banner.jpg"
    description: "The Confronting Climate Change is an annual public lecture series that brings together scientists, artists, policy experts, and community members to discuss our planet’s wellbeing and share solutions for our future."
    url: "https://calendar.ucsc.edu/event/confronting_climate_change_conference_-_community_fair#.YfrSAi-cbOQ"
  - title: "Cheers to 30 Years: Celebrating Alumni Supporting Students"
    date: "2022-04-23"
    starttime: "4:00pm"
    endtime: "6:00pm"
    image: "/assets/images/2021/seal-male.jpg"
    description: "The annual Beer & Wine Reception, celebrating the 30th anniversary of the Alumni Association Scholarship, on Saturday afternoon in the beautiful setting of Quarry Amphitheater. Sponsored by the Alumni Association."
    url: "https://calendar.ucsc.edu/event/elephant_seals_at_ucscs_ano_nuevo_reserve#.YGYLii2cbOS"
  - title: ' Keynote Lecture TBD'
    date: "2021-04-23"
    starttime: ""
    endtime: ""
    image: "/assets/images/2021/kraw-banner.jpg"
    description: "Details to come"
    url: "#"  

---

<div class="component-wrapper">
  <section class="content-centered">
    <div class="grid-container large">
        <h2>{{ page.title }}</h2>
        <p>Celebrating Alumni Voices with both virtual and in-person events—a mixtape of our favorite hits we've made just for you!</p>
    </div>
  </section>
</div>


<section class="heading">
  <h2 class="underline">Featured Events</h2>
</section>
<div class="events-card-list fade-out-siblings">
  {% for featured in page.featured %}
    <a class="events-card" href="{{ featured.url }}">
      <div class="events-card-content">
        <div class="date">
          <div class="month">{{ featured.date | date: "%b" }}</div>
          <div class="day">{{ featured.date | date: "%d" }}</div>
        </div>
          <div class="inner">
            <div class="image">
            <img src="{{ featured.image }}" alt="{{ featured.title }}"/>
            </div>
            <div class="card-content">
              <h4 class="header underline">{{ featured.title }}</h4>
              <p class="event-description">{{ featured.description }}</p>
            <div class="tags">
              <span class="topics-title">
                <div class="time">
                <i class="fa fa-clock-o turquiose-text"></i>{{ featured.date | date: "%A, %B %e, %Y" }} {% if featured.starttime != null %} at {% endif %}{{ featured.starttime }}
                {% if featured.endtime != null %} to {{ featured.endtime }} {% endif %}
                </div>
                <div class="location">
                  <i class="fa fa-map-marker turquiose-text"></i> Virtual Event
                </div>
              </span>
            </div>
          </div>
        </div>
      </div>
    </a>
  {% endfor %}
</div>
<!-- End three current events: Tag Home to display -->
<div class="more no-border">
  <a href="https://calendar.ucsc.edu/alumni_week" class="button primary">
    View more events
  </a>
</div>
