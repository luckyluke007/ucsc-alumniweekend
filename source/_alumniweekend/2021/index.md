---
layout: front-page
description: "Celebrating Alumni Week in true 2021 style. Have fun, remember your roots, reignite your passions, and connect like never before as our first virtual Alumni Week zooms you back to campus."

category: aw-2021

billboard:
  subtitle: "Monday-Sunday, April 19-25"
  image: /assets/images/2021/banner-image-v2.gif
  alt-text: "Alumni Week 2021 Arts"
  hero-title: "Alumni Week 2021"
  description: "Celebrating Alumni Week in true 2021 style. Have fun, remember your roots, reignite your passions, and connect like never before as our first virtual Alumni Week zooms you back to campus."
  action-text: Register Now
  register-url: '#'

featured:
  - title: "A conversation with Terri McCullough (Oakes '91, politics), chief of staff to Nancy Pelosi, in memory of Gabe Zimmerman (Stevenson '02, sociology)"
    date: "2021-04-24"
    starttime: "5:30pm"
    endtime: "7:00pm"
    image: "/assets/images/2021/terri-mccullough.jpg"
    description: "Gabe Zimmerman (Stevenson '02, sociology) was U.S. Congresswoman Gabby Giffords's community outreach director."
    url: "https://calendar.ucsc.edu/event/a_conversation_with_terri_mccullough_oakes_90_politics_chief_of_staff_to_nancy_pelosi_in_memory_of_gabe_zimmerman_stevenson_02_sociology#.YF1Y8i2cbOR"
  - title: "Visualizing Abolition: (Re)Enacting Revolution"
    date: "2021-04-20"
    starttime: "4:00pm"
    endtime: 
    image: "/assets/images/2021/va-banner.jpg"
    description: "Dread Scott's recent large-scale art project, Slave Rebellion Reenactment, was a community-engaged performance reenacting the largest rebellion of enslaved people in U.S. history. Prof. Gray, UC Davis, will join him in conversation about art, revolution, and reenactments."
    url: "https://calendar.ucsc.edu/event/visualizing_abolition_reenacting_revolution#.YEKdh5NKhH0"
  - title: "University Forum: The Filmmaker’s Voice in Changing Media Landscape"
    date: "2021-04-21"
    starttime: "5:30pm"
    endtime: 
    image: "/assets/images/2021/uf-banner.jpg"
    description: "Join us for an engaging conversation with award-winning filmmakers and professors in the Social Documentation MFA program Jacqueline Olive and Jennifer Maytorena Taylor, whose most recent feature documentaries are Always in Season and For the Love of Rutland."
    url: "https://calendar.ucsc.edu/event/university_forum_the_filmmakers_voice_in_changing_media_landscape#.YEZlxi9h3OR"
  - title: 'Live reading: “The Comedy of Errors”'
    date: "2021-04-23"
    starttime: "5:30pm"
    endtime: 
    image: "/assets/images/2021/comedy-errors-banner.jpg"
    description: "Watch a live reading of Shakespeare's masterful play “The Comedy of Errors” directed by theater arts professor Danny Scheie and featuring special guests, including illustrious alumni and fabulous friends."
    url: "https://calendar.ucsc.edu/event/live_reading_the_comedy_of_errors#.YEZluS9h3OR"
  - title: 'Kraw Lecture: The past, present, and future of DNA-based forensics'
    date: "2021-04-22"
    starttime: "5:30pm"
    endtime: "7:00pm"
    image: "/assets/images/2021/kraw-banner.jpg"
    description: "New technologies are being brought to bear in criminal justice. The existence of community databases of DNA information have enabled a new approach, forensic genetic genealogy, for identifying suspects in violent crimes."
    url: "https://calendar.ucsc.edu/event/kraw_lecture_the_past_present_and_future_of_dna-based_forensics#.YFjxqy2cbOR"
  - title: "Elephant Seals at UCSC's Año Nuevo Reserve"
    date: "2021-04-24"
    starttime: "10:00am"
    endtime: "11:00am"
    image: "/assets/images/2021/seal-male.jpg"
    description: "Join Reserve Director Patrick Robinson for a live view of the elephant seal colony at Año Nuevo."
    url: "https://calendar.ucsc.edu/event/elephant_seals_at_ucscs_ano_nuevo_reserve#.YGYLii2cbOS"
---

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

