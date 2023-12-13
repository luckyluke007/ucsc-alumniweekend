---
layout: front-page
title: "Save the date Alumni Reunion Weekend"
description: "Celebrating our Golden Slug alumni from the classes of 1963-1974."

category: "aw-2024"
order: 1
og-image: "https://alumniweekend.ucsc.edu/assets/images/2024/banner.png"

welcome:
  title: "Alumni Reunion Weekend"
  subhead: "Celebrating our Golden Slug alumni from the classes of 1963 - 1974."
  message: "This meaningful weekend will be filled with college-specific events and <br/>special moments to honor alumni celebrating their 50th or greater reunion milestones. <br/>We are excited to welcome these pioneers back to UC Santa Cruz for this special weekend."
  date: "Friday, April 12 - Saturday, April 13, 2024"

information:
  - title: "Volunteer"
    description: 'We have many <a href="https://alumni.ucsc.edu/volunteer/arw-volunteers.html">volunteer opportunities</a> for you to get involved now and during the weekend. <a href="https://docs.google.com/forms/d/e/1FAIpQLSe91dHZ5027XdMNNU__YX4gXrwRCdAH3tKNmfLz6kkxdz5bog/viewform">Sign-up to volunteer</a>.'
    image: '/assets/images/2023/volunteer-photo.jpg'
    layout: right
  - title: "Digital Memory Book"
    description: 'Share your UCSC memories and update classmates on where you are now. If you haven’t received an email invite to access the digital memory book, contact <a href="mailto:jmajane@ucsc.edu?subject=Digital%20Memory%20Book">Jesse Majane</a>.'
    image: '/assets/images/2023/share-photo-1.jpg' 
    layout: left
  - title: "Help Find Lost Alumni!"
    description: 'Over the years people move, change phone numbers, retire, create new email addresses and launch new social media profiles. We are asking for your help to find classmates we’ve lost touch with. If you have updated contact information for <a href="https://docs.google.com/spreadsheets/d/1_zyvwBJYMLJgws400imNdzGXCeQFGeYgqNrhnuLWTis/edit#gid=0">anyone on this list</a>, please reach out to <a href="mailto:alumni@ucsc.edu?subject=Help%20find%20lost%20alumni">alumni@ucsc.edu</a> so we can send them an invite to the weekend.'
    image: '/assets/images/2023/lost-alumni.jpg'
    layout: right

permalink: /

---

<img src="https://alumniweekend.ucsc.edu/assets/images/2024/banner.png" class="img-full" alt="UC Santa Cruz | Alumni: Alumni Reunion Weekend: April 14-15, 2023">
<section class="content-centered" style="padding: 0">
  <div class="grid-container large">
    <h1 style="font-size: 2em;"><strong>Save the Date<br />Alumni Reunion Weekend</strong></h1>
    <h2 style="font-size: 1.5em; display: block;"><strong>{{page.welcome.date}}</strong></h2>
    <span style="font-size: 1.35em; display: block;">{{page.welcome.subhead}}</span>
    <p class="lead" style="margin-top: 1em;"> {{page.welcome.message}}</p>
    <h3>Registration coming soon</h3>
  </div>
</section>



<style>
  .page-utilities {
    display: none;
  }
</style>


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