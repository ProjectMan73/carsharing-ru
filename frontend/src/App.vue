<template>
  <v-app>
    <v-main>
      <sidebar/>
      <the-header/>
      <the-footer/>
      <the-slider/>
      <router-view/>
    </v-main>
  </v-app>
</template>

<script>
import Sidebar from '@/components/Sidebar.vue';
import TheFooter from '@/views/TheFooter.vue';
import TheHeader from '@/views/TheHeader.vue';
import TheSlider from '@/views/TheSlider.vue';

export default {
  name: 'App',
  components: {
    Sidebar, TheFooter, TheHeader, TheSlider,
  },
  data: () => ({
    //
  }),
};
</script>
<style scoped="scss">
v-app {
  min-height: 100vh;
  display: flex;
  flex-direction: row;
  overflow-y: visible;
}
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Roboto', sans-serif;
 }
h1{
  position: absolute;
  width: 192px;
  height: 32px;
  left: 128px;
  top: 32px;

  font-family: Roboto;
  font-style: normal;
  font-weight: bold;
  font-size: 30px;
  line-height: 35px;

  /* Main accent */
  color: #0EC261;

}
</style>
