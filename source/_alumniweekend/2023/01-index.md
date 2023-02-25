---
layout: front-page
title: Alumni Reunion Weekend
description: "Alumni Reunion Weekend will celebrate our Golden Slug alumni from the classes of 1965-1973."

category: "aw-2023"
order: 1
og-image: "https://alumniweekend.ucsc.edu/assets/images/2023/og-image.jpg"

featured:
  - title: 'Class of ‘73 Virtual Kick-Off, How We’re Still Changing the World'
    date: "2023-04-13"
    starttime: "5:30pm"
    endtime: "7:00pm"
    location: "Virtual Event"
    image: "/assets/images/2022/trivia-night-featured.jpg"
    description: "As the Class of ’73 celebrates its 50th anniversary, classmates will come together to reflect on how they are still changing the world. Hear and share about how the Class of ’73 has been at the forefront of progress over the past 50 years. Come celebrate the transformative impact of fellow classmates and colleagues."
    url: "/alumniweekend/2023/events#featured-1"
  - title: '50+ Year Reunion Celebrating and honoring our Golden Slug alumni from the classes of 1965-1973 Stevenson Events Center'
    date: "2023-04-14"
    starttime: "6:00pm"
    endtime: "9:00pm"
    location: "Stevenson Event Center"
    image: "/assets/images/2022/trivia-night-featured.jpg"
    description: "This is the weekend’s main event where alumni from graduating classes 1965 to 1973 will gather together to celebrate their milestone reunion. Alumni will be presented with the distinct recognition for their part in the history of UC Santa Cruz."
    url: "/alumniweekend/2023/events#featured-2"
  - title: 'College Gatherings'
    date: "2023-04-15"
    starttime: ""
    endtime: ""
    location: "Stevenson Event Center"
    image: "/assets/images/2022/trivia-night-featured.jpg"
    description: "Attend one of the many college hosted events to gather with classmates from your college in the libraries, dining halls and lounges you once called home. Review the full event listings to see events organized by college."
    url: "/alumniweekend/2023/events#featured-3"
  - title: 'Then and Now Rolling Tours of UCSC'
    date: "2023-04-15"
    starttime: "1:00pm"
    endtime: "3:00pm"
    location: "Meet in the Cowell Circle "
    image: "/assets/images/2022/trivia-night-featured.jpg"
    description: "Hop aboard and join Larry Pageler (Crown, ’77) on a driving tour of campus to learn campus history, explore what is new and reminisce about our time as students."
    url: "/alumniweekend/2023/events#featured-4"


welcome:
  title: "Alumni Reunion Weekend"
  message: "Alumni Reunion Weekend will celebrate our Golden Slug alumni from the classes of 1965-1973. This meaningful weekend will be filled with college-specific events and special moments to honor alumni celebrating their 50th or greater reunion milestones. We are excited to welcome these pioneers back to UC Santa Cruz for this special weekend."
  date: "Friday, April 14 - Saturday, April 15, 2023"

information:
  - title: "Volunteer"
    description: 'We have many <a href="https://alumni.ucsc.edu/volunteer/arw-volunteers.html">volunteer opportunities</a> for you to get involved now and during the weekend. <a href="https://docs.google.com/forms/d/e/1FAIpQLSe91dHZ5027XdMNNU__YX4gXrwRCdAH3tKNmfLz6kkxdz5bog/viewform">Sign-up to volunteer</a>.'
    image: '/assets/images/2023/volunteer-photo.jpg'
    layout: right
  - title: "Share Your UCSC Photos"
    description: 'We will be building a special photo wall compiled of images you and your classmates send in from your student days on campus as a student at UCSC. Please email us your photos in any format to <a href="mailto:alumni@ucsc.edu">alumni@ucsc.edu</a>.'
    image: '/assets/images/2023/share-photo-1.jpg' 
    layout: left


permalink: /alumniweekend/2023/

---


<style>
  .page-utilities {
    display: none;
  }
</style>


<section class="heading">
  <h2 class="underline">Highlighted Events</h2>
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
                  <i class="fa fa-map-marker turquiose-text"></i> {{ featured.location }}
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
  <a href="/alumniweekend/2023/events" class="button primary">
    View more events
  </a>
</div>


{% for information in page.information %}
<section class="content-w-media {{ information.layout }}">
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



