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
            <b-carousel-slide img-src="@/static/delhaizebio3.png"></b-carousel-slide>
            <b-carousel-slide img-src="@/static/delhaize365-2.png"></b-carousel-slide>
                
            <!-- <b-carousel-slide><img-lazy slot="img" class="d-block img-fluid w-100" width="1024" height="480"
             src="@/static/delhaize3.png" alt="image slot"></img-lazy></b-carousel-slide>
            <b-carousel-slide><img-lazy slot="img" class="d-block img-fluid w-100" width="1024" height="480"
             src="@/static/delhaize1.png" alt="image slot"></img-lazy></b-carousel-slide> -->
        </b-carousel>
        <div class="wrap">
            <h2>Delhaize Bio and 365</h2>
            <p class="desc">
                In 2019 and 2020 I was working at <a href="https://www.sunny-side-up.be" target="blank">Sunny Side Up</a> studio, where I mostly worked on packaging design and pre-press for Delhaize Bio and Delhaize 365 products. Following a strict guideline and versioning system set out by Delhaize marketing team. <br>During that period I occasionally worked on some book design and photo-editing for Sunny Side Up's other projects too.
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