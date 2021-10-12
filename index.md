<button @click="$refs.myVueperSlides[`${autoPlaying ? 'pause' : 'resume'}Autoplay`]();autoPlaying = !autoPlaying">
  {{ autoPlaying ? 'Pause' : 'Resume' }}
</button>
<button @click="pauseOnHover = !pauseOnHover">Pause on mouseover</button>
<code>Currently {{ internalAutoPlaying ? 'playing' : 'paused' }}</code>

<vueper-slides
  ref="myVueperSlides"
  autoplay
  :pause-on-hover="pauseOnHover"
  @autoplay-pause="internalAutoPlaying = false"
  @autoplay-resume="internalAutoPlaying = true">
  <vueper-slide
    v-for="(slide, i) in slides"
    :key="slide.id"
    :title="slide.title"
    :content="slide.content"
    :style="'background-color: ' + colors[i % 4]" />
  <template #pause>
    <i class="icon pause_circle_outline"></i>
  </template>
</vueper-slides>

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
  
