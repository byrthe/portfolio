<template>
    <div class="b-row project" style="border-top:none!important; padding-top:0;">
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
            <b-carousel-slide img-src="@/static/bday2.png"></b-carousel-slide>
            <b-carousel-slide img-src="@/static/bday1.png"></b-carousel-slide>
                
        </b-carousel>
        <div class="wrap">
            <h2>Queer of Hearts</h2>
            <p class="desc">
                Am invitation shaped like a playing card for my own damn 30th birthday.
            </p>
            <div class="tags">
                <p class="tag">design</p>
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