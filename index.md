<button @click="parallax *= -1;$refs.myVueperSlides.refreshParallax()">
  reverse parallax effect
</button>
<button @click="parallaxFixedContent = !parallaxFixedContent">
  Add a fix title
</button>

<vueper-slides ref="myVueperSlides" :parallax="parallax" :parallax-fixed-content="parallaxFixedContent">
  <vueper-slide
    v-for="(slide, i) in slides" :key="i"
    :image="slide.image"
    :title="parallaxFixedContent ? slide.title : ''"
    :content="parallaxFixedContent ? slide.content : ''" />
</vueper-slides>

---
layout: splash
feature_row:
  - title: "Resources"
    excerpt: "Learn more about the available resources!"
    url: "/empowering-you/"
    btn_label: "Read More"
    btn_class: "btn--inverse"
  - title: "Projects"
    excerpt: "Learn more about our projects!"
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
  
