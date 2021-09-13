<template>
    <div>
        <div class="b-row">
            <h2>+32</h2>
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
                <b-carousel-slide img-src="@/static/+32_triPostal_fb.jpg"></b-carousel-slide>
                <b-carousel-slide img-src="@/static/+32_triPostal_insta.jpg"></b-carousel-slide>
                     
            </b-carousel>
            <p class="desc">
                short project description
            </p>
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
body{
    background-color: black;
}
.wrapper{
    height: 500px!important;
}
.carousel{
    border: 1px solid orange;
    
}
.carousel-inner{
    position: relative;
    height:500px;
    width: auto;
}
.carousel-item img{
    height:500px;
    width: auto;
}
.carousel .item {
  height: 300px;
}
</style>