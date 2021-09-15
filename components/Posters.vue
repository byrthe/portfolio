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
            <b-carousel-slide img-src="@/static/dziri1.png"></b-carousel-slide>
            <b-carousel-slide img-src="@/static/dziri2.png"></b-carousel-slide>
            <b-carousel-slide img-src="@/static/dziri3.png"></b-carousel-slide> 
                
        </b-carousel>
        <div class="wrap">
            <h2>Dziri</h2>
            <p class="desc">
                Poster proposal for dj and producer Dziri. Dziri asked for tour posters that would involve an abstraction of an eye. I proposed these sequential series of iris patterns that would accumulate in the poster design over time. Unfortunately the project was not excecuted.
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