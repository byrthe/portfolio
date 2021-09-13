<template>
    <div>
        <div class="b-row">
            <h2>Get Lost - art route</h2>
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
                <b-carousel-slide img-src="@/static/getlost-artroute1.png"></b-carousel-slide>
                <b-carousel-slide img-src="@/static/getlost-artroute2.png"></b-carousel-slide>
                <b-carousel-slide img-src="@/static/getlost-artroute3.png"></b-carousel-slide>
                <b-carousel-slide img-src="@/static/getlost-artroute4.png"></b-carousel-slide>
                <b-carousel-slide img-src="@/static/getlost-artroute5.png"></b-carousel-slide>      
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
}
.carousel-item img{
    /* height: 75vh!important;
    width: auto; */
}
.carousel .item {
  height: 300px;
}
</style>