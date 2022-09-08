<template>
  <div class="d-flex px-3">
    <div class="mr-3 feature-left">
      <div role="button" :class="`${item.maintained ? 'feature-img-container' : ''} position-relative mb-3`" v-for="item in icons" :key="item.id">
        <img class="img-fluid" :src="getImgUrl(item.url)" :alt="`Featurss${item.id}`" :title="item.name">
      </div>
    </div>

    <div>
        <div role="button" :class="`${item.maintained ? 'feature-img-container' : ''} position-relative mb-3`" v-for="item in images" :key="item.id">
          <img class="img-fluid" :src="getImgUrl(item.url)" :alt="`Featurss${item.id}`">
          <button v-if="item.maintained" class="feature-btn">Maintained</button>
        </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data() {
    return {
      icons: [
        { id: 1, name: 'Used', url: "used.png" },
        { id: 2, name: 'Live', url: "live.png" },
        { id: 3, name: 'Sport', url: "sport.png" },
        { id: 4, name: 'Lottery', url: "lottery.png" },
        { id: 5, name: 'Poker', url: "poker.png" },
        { id: 6, name: 'Game', url: "game.png" },
      ],
      images: [
        { id: 1, url: "feature1.png", maintained: true },
        { id: 2, url: "feature2.png", maintained: false },
        { id: 3, url: "feature3.png", maintained: false },
        { id: 4, url: "feature4.png", maintained: false },
      ],
    }
  },
  methods: {
    getImgUrl: function (imagePath) {
      return require('@/assets/images/features/' + imagePath);
    },
  }
}
</script>

<style scoped>
.feature-img-container {
  transition: 0.3s ease-in all;
}

.feature-img-container:before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  bottom: 0;
  right: 0;
  background-color: rgba(0, 0, 0, 0.7);
}

.feature-btn {
  background-color: rgb(0, 0, 0, 0.6);
  border-radius: 26px;
  padding: 10px 50px;
  color: #bda8a8;
  border: 0;
  z-index: 3;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}

@media screen and (max-width: 500px) {
  .feature-left img {
    width: 90%;
  }
}
</style>
