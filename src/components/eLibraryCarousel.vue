<template>
  <div>
    <b-carousel
      id="carousel-1"
      v-model="slide"
      :interval="4000"
      controls
      indicators
      background="#ababab"
      img-width="1024"
      img-height="480"
      style="text-shadow: 1px 1px 2px #333;"
      @sliding-start="onSlideStart"
      @sliding-end="onSlideEnd"
    >
      <!-- Text slides with image -->
      <b-carousel-slide
        img-src="https://th.bing.com/th/id/R2d0fe4fa065f6e9f79bfd41c7c6ff0bb?rik=wCOoY9AAnzKVbw&riu=http%3a%2f%2fstatic.guim.co.uk%2fsys-images%2fGuardian%2fPix%2fpictures%2f2015%2f2%2f20%2f1424454392161%2fLibrary-books-009.jpg&ehk=YRW0r03p0QhBH0w4oDvu6DznESrPPixLJsLHOPzcex4%3d&risl=&pid=ImgRaw"
      ></b-carousel-slide>

      <!-- Slides with custom text -->
      <b-carousel-slide img-src="https://i.cbc.ca/1.1229449.1378976415!/httpImage/image.jpg_gen/derivatives/16x9_780/hi-852-generic-books-8col.jpg">
      </b-carousel-slide>

      <!-- Slides with image only -->
      <b-carousel-slide img-src="https://media.npr.org/assets/img/2016/08/08/gettyimages-175590398_wide-30355c6f6fe56c3907759582f4e7e8a81f7fc41c.jpg?s=1400"></b-carousel-slide>

      <!-- Slides with img slot -->
      <!-- Note the classes .d-block and .img-fluid to prevent browser default image alignment -->
      <b-carousel-slide>
        <template #img>
          <img
            class="d-block img-fluid w-100"
            width="500"
            height="480"
            src="https://c2.staticflickr.com/4/3026/2549674908_2259c9b26d_b.jpg"
            alt="image slot"
          >
        </template>
      </b-carousel-slide>

      <!-- Slide with blank fluid image to maintain slide aspect ratio -->
      <b-carousel-slide caption="Blank Image" img-blank img-alt="Blank image">
      </b-carousel-slide>
    </b-carousel>

    <p class="mt-4">
      Slide #: {{ slide }}<br>
      Sliding: {{ sliding }}
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
      onSlideStart() {
        this.sliding = true
      },
      onSlideEnd() {
        this.sliding = false
      }
    }
  }
</script>