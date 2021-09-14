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
            <b-carousel-slide img-src="@/static/skillbank1.png"></b-carousel-slide>
            <b-carousel-slide img-src="@/static/skillbank2.png"></b-carousel-slide>      
        </b-carousel>
        <h2>Skill Bank</h2>
        <p class="desc">
            A prototype for a skill sharing website. I made this website as a try-out project, to learn how to work with databases (sql3) and node.js. The site is currently not deployed nor responsive, but the repo can be found here on <a href="https://github.com/byrthe/skillBankApp" target="blank">github</a>. 
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