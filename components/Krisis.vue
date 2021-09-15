<template>
    <div class="b-row project">
        <b-carousel
        id="carousel-1"
        v-model="slide"
        :interval="0"
        controls
        background="transparent"
        class="d-inline-block"
        img-height="500px"
        @sliding-start="onSlideStart"
        @sliding-end="onSlideEnd"
        >
            <b-carousel-slide img-src="@/static/krisis1.png"></b-carousel-slide>
            <b-carousel-slide img-src="@/static/krisis4.png"></b-carousel-slide>
            <b-carousel-slide img-src="@/static/krisis5.png"></b-carousel-slide>
            <b-carousel-slide img-src="@/static/krisis2.png"></b-carousel-slide>
            <b-carousel-slide img-src="@/static/krisis3.png"></b-carousel-slide>
  
        </b-carousel>
        <div class="wrap">
            <h2>Krisis - philosophy journal</h2>
            <p class="desc">
                Krisis is a philosophy journal affiliated with the University of Amsterdam.
                In 2016 Krisis was publishing only on paper, and an occasional article online. I designed a new (very clear and to the point) environment for them, in which they could slowly digitize their entire archive and where it would be accessible from any platform. <br>
                As they depended on a specific plugin, that allowed them to peer-review their articles, we were bound to use Wordpress. The development was done in collaboration with Frank Molenaar. <a href="https://archive.krisis.eu/" target="blank">An archived version of that site is available here</a>.
            </p>
            <div class="tags">
                <p class="tag">design</p>
                <p class="tag">development</p>

            </div>
        </div>
    </div>
</template>

<script>
export default {
    data() {
      return {
        slide: 0,
        sliding: null
      }
    },
    methods: {
      onSlideStart(slide) {
        this.sliding = true
      },
      onSlideEnd(slide) {
        this.sliding = false
      }
    }
  }
</script>

<style>

</style>