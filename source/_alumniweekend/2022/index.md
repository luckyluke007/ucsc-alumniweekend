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
  - title: 'Banana Slug Trivia Night!'
    date: "2022-04-19"
    starttime: "6:00pm"
    endtime: "7:00pm"
    image: "/assets/images/2022/trivia-night-featured.jpg"
    description: "A virtual trivia night for all alumni."
    url: "https://calendar.ucsc.edu/event/banana_slug_trivia_night_117#.Ygv8Dy-cbOQ"
  - title: "Global data, personal stories: Journalists documenting the COVID-19 pandemic"
    date: "2022-04-19"
    starttime: "5:30pm"
    endtime: "7:00pm"
    image: "/assets/images/2022/uf-banner.jpg"
    description: "Journalism has been critical to helping society understand and react to the COVID pandemic, which has spurred an unprecedented demand for accurate science communication. But how do journalists separate facts from misinformation when scientific knowledge changes constantly? And how do journalists remain focused when themselves living through the disruption of the pandemic? Two alums of UC Santa Cruz's prestigious Science Communication Program share what they have learned by covering the biggest science and health story of our lifetimes."
    url: "https://calendar.ucsc.edu/event/university_forum_featuring_julia_calderone_nicholas_st_fleur#.Yg0spS-cbOQ"
  - title: "Art at Work in the World: Justice, Decolonization, and Collaboration in the New EASP MFA"
    date: "2022-04-20"
    starttime: "5:30pm"
    endtime: "7:00pm"
    image: "/assets/images/2022/uf-banner.jpg"
    description: "Art, the systems and institutions that surround and support art, and the people who make art are constantly evolving in relation to worlds in flux. In these uncertain times of climate crisis and of the persistence of extreme racial and other social inequities, art’s boundary-crossing, associative and connective possibilities can reach across perceived divisions and create new forms for understanding and action. Tonight, we share with you a few examples of some of the practice-based research projects already underway among our first cohort of our new Graduate MFA in Environmental Art and Social Practice."
    url: "https://calendar.ucsc.edu/event/university_forum_with_arts_dean_celine_parreas_shimizu#.Yg0s9S-cbOQ"
  - title: "Strange Weather Alumni Reception at the MAHss"
    date: "2022-04-22"
    starttime: "6:00pm"
    endtime: "8:00pm"
    image: "/assets/images/2022/mah-featured.jpg"
    description: "Join us at the Santa Cruz Museum of Art & History for refreshments, mingling, and viewing the exhibit Strange Weather, which brings together works by influential artists from the 20th and 21st century that creatively illuminate and reframe the boundaries of bodies and the environment."
    url: "https://calendar.ucsc.edu/event/strange_weather_alumni_reception_at_the_mah#.YfrRfS-cbOQ"
  - title: 'Confronting Climate Change Conference - Community Fair'
    date: "2022-04-23"
    starttime: "10:00am"
    endtime: "4:00pm"
    image: "/assets/images/2022/climate-conference.jpg"
    description: "The Confronting Climate Change is an annual public lecture series that brings together scientists, artists, policy experts, and community members to discuss our planet’s wellbeing and share solutions for our future."
    url: "https://calendar.ucsc.edu/event/confronting_climate_change_conference_-_community_fair#.YfrSAi-cbOQ"
  - title: "Cheers to 30 Years: Celebrating Alumni Supporting Students"
    date: "2022-04-23"
    starttime: "4:00pm"
    endtime: "6:00pm"
    image: "/assets/images/2022/alumni-week-art-featured.jpg"
    description: "Cheers to 30 years! Celebrating three decades of alumni supporting students. Join us for our annual Alumni Week reception, celebrating the 30th anniversary of the Alumni Association Scholarship, on Saturday afternoon in the beautiful setting of the Cowell Courtyard. Sponsored by the Alumni Association."
    url: "https://calendar.ucsc.edu/event/elephant_seals_at_ucscs_ano_nuevo_reserve#.YGYLii2cbOS"

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
