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
            <b-carousel-slide img-src="@/static/sotu1.png"></b-carousel-slide>
            <b-carousel-slide img-src="@/static/sotu2.png"></b-carousel-slide>
            <b-carousel-slide img-src="@/static/sotu3.png"></b-carousel-slide>

                
        </b-carousel>
        <div class="wrap">
            <h2>Sounds Of The Underground Festival</h2>
            <p class="desc">
                Posters for the underground noise music festival 'Sounds Of The Undergroud'. The posters are made stereo scopic, drawing in the popular <a href="https://en.wikipedia.org/wiki/Autostereogram" target="blank">'magic eye'</a> books from the 90's. If you stare at the poster as if looking through a window, a 3D image of a ladder descending in a well, appears through the noise. <br>
                In collaboration with Karoline Swiezynski. Screenprinted by us in 4 colors at AGA Lab.
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