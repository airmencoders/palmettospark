---
layout: splash
feature_row:
  - title: "Projects"
    excerpt: "Learn more about our projects."
    url: "/projects/"
    btn_label: "Go to Projects"
    btn_class: "btn--inverse"
  - title: "Press"
    excerpt: "Read more about Palmetto Spark in the news."
    url: "/press/"
    btn_label: "Read More"
    btn_class: "btn--inverse"
  - title: "Submit Ideas"
    excerpt: "Submit innovation ideas to receive help and SIF."
    url: "https://forms.gle/e38rXYHrn9fWLFHs5"
    btn_label: "Submit Now"
    btn_class: "btn--inverse"
---
  
<br /><br />
> "Give Airmen an inch...and we will return a mile!" 


<br /><br />
{% include feature_row %}
  
<h3 class="archive__subtitle">{{ site.data.ui-text[site.locale].recent_posts | default: "Recent Posts" }}</h3>

{% if paginator %}
  {% assign posts = paginator.posts %}
{% else %}
  {% assign posts = site.posts %}
{% endif %}

{% for post in posts %}
  {% include archive-single.html %}
{% endfor %}

{% include paginator.html %}

![Your base needs you ... to submit your ideas](https://github.com/airmencoders/palmettospark/blob/master/3ukqu9.jpg?raw=true)
### [Submit an Idea via IdeaScale (CAC Required)](https://usaf.ideascalegov.com/a/ideas/recent/campaign-filter/byids/campaigns/143/stage/unspecified)
### [Submit an Idea (No CAC)](https://forms.gle/e38rXYHrn9fWLFHs5) 

## COVID-19 Resources:
* [Telework & Network Updates (CAC Requried)](https://www.my.af.mil/gcss-af/USAF/ep/globalTab.do?channelPageId=sE66807CD6D089CAC016D1CE8DE3E003C)

## Useful Links:
* [AFWERX](https://afwerx.af.mil)
* [CPI](https://static.e-publishing.af.mil/production/1/saf_mg/publication/afi38-401/afi38-401.pdf)
* [AF Software Efforts](https://software.af.mil)