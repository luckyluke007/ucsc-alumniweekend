---
title: "Banana Slug Share Sessions"
description: 'As UC alumni, we want to ensure that the programs and activities that make the UC Santa Cruz experience so unique have the resources they need to remain resilient. We know the experience that each of us had on campus made a profound impact on our lives. Join thousands of dedicated alumni like you by making a donation to UC Santa Cruz, ensuring our future alumni have the support they need to thrive.'
layout: 2021/page
order: 2

published: true
---
{: .underline}
## {{ page.title }}

{% assign eventdate = site.data.share-sessions %}
<h3>{{ eventdate }}</h3>
{% for event in site.data.share-sessions %}
  <div class="component-wrapper">
    <a class="events-card" href="{{ event.zoom-link }}">
      <div class="events-card-content">
        <div class="date">
            <div class="month">{{ event.date | date: "%b" }}</div>
            <div class="day">{{ event.date | date: "%d" }}</div>
        </div>
          <div class="inner">
            <div class="card-content">
              <h4 class="header">{{ event.event }}</h4>
              <div class="tags">
                <span class="topics-title">
                  <div class="time">
                      <i class="fa fa-clock-o turquiose-text"></i> {{ event.date | date: "%A, %B %e, %Y" }} at {{ event.start }} to {{ event.end }}
                  </div>
                  <div class="location">
                    <i class="fa fa-map-marker turquiose-text"></i> Virtual
                  </div>
                </span>
              </div>
            </div>
          </div>   
      </div>
    </a>
  </div>
{% endfor %}




