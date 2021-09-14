<template>
    <div class="b-row project" style="border-top:none!important">
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
            <b-carousel-slide img-src="@/static/getlost-artroute3.png"></b-carousel-slide>
            <b-carousel-slide img-src="@/static/getlost-artroute4.png"></b-carousel-slide>
            <b-carousel-slide img-src="@/static/getlost-artroute5.png"></b-carousel-slide> 
            <b-carousel-slide img-src="@/static/getlost-artroute1.png"></b-carousel-slide>
            <b-carousel-slide img-src="@/static/getlost-artroute2.png"></b-carousel-slide>
                 
        </b-carousel>
        <h2>Get Lost - art route</h2>
        <p class="desc">
            Full visual identity for art route Get Lost consisting of posters, catalogues, website and promotional material. The identity is based on the high rises that make up the decor for this art route, and is playing with the shift in focus of looking through a window or seeing the reflections in it. <br>
            Design in collaboration with Karoline Swiezyinski. Development in collaboration with Joel Galvez. Printing by Coers&Roest.
        </p>
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