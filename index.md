---
layout: splash
feature_row:
  - title: "Resources"
    excerpt: "Learn more about the resources available to you."
    url: "/empowering-you/"
    btn_label: "Read More"
    btn_class: "btn--inverse"
  - title: "Projects"
    excerpt: "Learn more about our projects."
    url: "/projects/"
    btn_label: "Go to Projects"
    btn_class: "btn--inverse"
  - title: "Pitch Day"
    excerpt: "Submit your ideas to accelerate change!"
    url: "https://forms.gle/e38rXYHrn9fWLFHs5"
    btn_label: "Submit Now"
    btn_class: "btn--inverse"
---
  
  <br /><br />
![](/assets/images/welcome.png){: .align-center}
 
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
