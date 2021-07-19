<template>
  <div class="the-slider">
    <v-carousel v-model="model" class="v-carousel"
                height="100%"
                delimiter-icon="mdi-checkbox-blank-circle"
                hide-delimiter-background
                prev-icon="mdi-chevron-left"
                next-icon="mdi-chevron-right"
                >
      <v-carousel-item
        v-for="(item,i) in items"
        :key="i"
        :src="item.src"
      ></v-carousel-item>
    </v-carousel>
  </div>
</template>

<script>
export default {
  name: 'TheSlider',
  data() {
    return {
      items: [
        {
          src: '/assets/jp-valery-1052513-unsplash.jpg',
        },
        {
          src: 'https://cdn.vuetifyjs.com/images/carousel/sky.jpg',
        },
        {
          src: 'https://cdn.vuetifyjs.com/images/carousel/bird.jpg',
        },
        {
          src: 'https://cdn.vuetifyjs.com/images/carousel/planet.jpg',
        },
      ],
    };
  },
};
</script>

<style scoped="scss">
.the-slider{
  position: absolute;
  width: 688px;
  height: 100%;
  left: 752px;
  top: 0px;
  background: linear-gradient(180deg, rgba(0, 0, 0, 0) 0%, #000000 100%);
  mix-blend-mode: normal;
}
</style>
