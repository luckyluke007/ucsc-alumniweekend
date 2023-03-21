---
layout: front-page
title: Alumni Reunion Weekend
description: "Alumni Reunion Weekend will celebrate our Golden Slug alumni from the classes of 1965-1973."

category: "aw-2023"
order: 1
og-image: "https://alumniweekend.ucsc.edu/assets/images/2023/og-image.jpg"

welcome:
  title: "Alumni Reunion Weekend"
  subhead: "Celebrating our Golden Slug alumni from the classes of 1965-1973."
  message: "This meaningful weekend will be filled with college-specific events and <br/>special moments to honor alumni celebrating their 50th or greater reunion milestones. <br/>We are excited to welcome these pioneers back to UC Santa Cruz for this special weekend."
  date: "Friday, April 14 - Saturday, April 15, 2023"

featured:
  - title: 'Class of ‘73 Virtual Kick-Off, How We’re Still Changing the World'
    date: "2023-04-13"
    time: "5:30 - 7:00 p.m."
    location: "Virtual Event"
    image: "/assets/images/2023/class-73.jpg"
    description: "As the Class of ’73 celebrates its 50th anniversary, classmates will come together to reflect on how they are still changing the world. Hear and share about how the Class of ’73 has been at the forefront of progress over the past 50 years. Come celebrate the transformative impact of fellow classmates and colleagues."
    url: "/alumniweekend/2023/events#featured-1"
  - title: '50+ Year Reunion Celebrating and honoring our Golden Slug alumni from the classes of 1965-1973 Stevenson Events Center'
    date: "2023-04-14"
    time: "6:00 - 9:00pm"
    location: "Stevenson Event Center"
    image: "/assets/images/2023/50-celebration.jpg"
    description: "This is the weekend’s main event where alumni from graduating classes 1965 to 1973 will gather together to celebrate their milestone reunion. Alumni will be presented with the distinct recognition for their part in the history of UC Santa Cruz."
    url: "/alumniweekend/2023/events#featured-2"
  - title: 'College Gatherings'
    date: "2023-04-15"
    starttime: ""
    endtime: ""
    location: "Colleges"
    image: "/assets/images/2023/college-gathering.jpg"
    description: "Attend one of the many college hosted events to gather with classmates from your college in the libraries, dining halls and lounges you once called home. Review the full event listings to see events organized by college."
    url: "/alumniweekend/2023/events#featured-3"
  - title: 'Then and Now Rolling Tours of UCSC'
    date: "2023-04-15"
    time: "10:00 - 1:00 p.m. and 1:00 p.m. - 3:00 p.m."
    location: "Meet in the Cowell Circle "
    image: "/assets/images/2023/then-now-tours.jpg"
    description: "Hop aboard and join Larry Pageler (Crown, ’77) on a driving tour of campus to learn campus history, explore what is new and reminisce about our time as students."
    url: "/alumniweekend/2023/events#featured-4"

information:
  - title: "Volunteer"
    description: 'We have many <a href="https://alumni.ucsc.edu/volunteer/arw-volunteers.html">volunteer opportunities</a> for you to get involved now and during the weekend. <a href="https://docs.google.com/forms/d/e/1FAIpQLSe91dHZ5027XdMNNU__YX4gXrwRCdAH3tKNmfLz6kkxdz5bog/viewform">Sign-up to volunteer</a>.'
    image: '/assets/images/2023/volunteer-photo.jpg'
    layout: right
  - title: "Digital Memory Book"
    description: 'Share your UCSC memories and update classmates on where you are now. If you haven’t received an email invite to access the digital memory book, contact <a href="mailto:kjudd@ucsc.edu?subject=Digital%20Memory%20Book">Kayla Judd</a>.'
    image: '/assets/images/2023/share-photo-1.jpg' 
    layout: left
  - title: "Help Find Lost Alumni!"
    description: 'Over the years people move, change phone numbers, retire, create new email addresses and launch new social media profiles. We are asking for your help to find classmates we’ve lost touch with. If you have updated contact information for <a href="https://docs.google.com/spreadsheets/d/1_zyvwBJYMLJgws400imNdzGXCeQFGeYgqNrhnuLWTis/edit#gid=0">anyone on this list</a>, please reach out to <a href="mailto:alumni@ucsc.edu?subject=Help%20find%20lost%20alumni">alumni@ucsc.edu</a> so we can send them an invite to the weekend.'
    image: '/assets/images/2023/lost-alumni.jpg'
    layout: right


permalink: /

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
                <i class="fa fa-clock-o turquiose-text"></i> {{ featured.date | date: "%A, %B %e, %Y" }} {% if featured.time != null %} at {{ featured.time }} {% endif %}
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