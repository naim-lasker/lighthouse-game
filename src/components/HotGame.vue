<template>
  <div class="hotgame-container pt-2 pl-3">
    <h6>Hot Game</h6>
    <carousel :settings="settings">
      <slide v-for="item in images" :key="item.id">
        <img role="button" :src="getImgUrl(item.url)" :alt="item.url">
      </slide>
    </carousel>
  </div>
</template>

<script>
import 'vue3-carousel/dist/carousel.css';
import { Carousel, Slide } from 'vue3-carousel';

export default {
  name: 'HotGame',
  components: {
    Carousel,
    Slide,
  },
  data() {
    return {
      images: [
      { id: 1, url: "hotgame1.png" },
      { id: 2, url: "hotgame3.png" },
      { id: 3, url: "hotgame1.png" },
      { id: 4, url: "hotgame4.png" },
      { id: 5, url: "hotgame2.png" },
      { id: 6, url: "hotgame1.png" },
      { id: 7, url: "hotgame2.png" },
      { id: 8, url: "hotgame3.png" },
      { id: 9, url: "hotgame2.png" },
      { id: 10, url: "hotgame3.png" },
      { id: 11, url: "hotgame1.png" },
      { id: 12, url: "hotgame3.png" },
    ],
    
    settings: {
        itemsToShow: 4.8,
        breakpoints: {
          300: {
            itemsToShow: 1.5,
          },
          320: {
            itemsToShow: 2,
          },
          360: {
            itemsToShow: 2.3,
          },
          400: {
            itemsToShow: 2.5,
          },
          460: {
            itemsToShow: 2.9,
          },
          520: {
            itemsToShow: 3.5,
          },
          600: {
            itemsToShow: 3.5,
          },
          670: {
            itemsToShow: 4.5,
          },
        },
      },
    }
  },
  methods: {
    getImgUrl: function (imagePath) {
      return require('@/assets/images/hotgame/' + imagePath);
    }
  }
}
</script>

<style scoped>
.hotgame-container {
  background-color: #0F0F0F;
}
</style>
