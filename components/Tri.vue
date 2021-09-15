<template>

    <div class="b-row project">
        <b-carousel
        id="carousel-1"
        v-model="slide"
        :interval="0"
        controls
        background="transparent"
        class="d-inline-block"
        @sliding-start="onSlideStart"
        @sliding-end="onSlideEnd"
        >
            <div class="carousel-inner" role="listbox">
                <b-carousel-slide img-src="@/static/+32_triPostal_insta.png"></b-carousel-slide>
                <b-carousel-slide img-src="@/static/+32_triPostal_fb.png"></b-carousel-slide>
            </div>
                    
        </b-carousel>
        <div class="wrap">
            <h2>+32</h2>
            <p class="desc">
                A digital flyer (for facebook and instagram) for the +32 collective, hosting a night at Tri Postal in Brussels. The flyer should give an impression of what you can find in the bottom of your bag after a +32 party night. The event was at full capacity :-) 
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