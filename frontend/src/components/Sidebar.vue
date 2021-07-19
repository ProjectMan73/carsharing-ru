<template>
  <div class="sidebar">
  <v-app id="inspire">
    <v-navigation-drawer
      app
      color="#151B1F"
      width="64"
    >
      <v-icon class="nav-btn" v-if="!show" @click="show = !show" key="menu">mdi-menu</v-icon>
      <v-icon class="nav-btn" v-else @click="show = !show" key="close">mdi-close</v-icon>
    </v-navigation-drawer>
    <transition name="fade">
      <ul v-if="show">
        <li v-for="item in items" v-bind:key="item">{{item}}</li>
      </ul>
      <v-icon></v-icon>
    </transition>
  </v-app>
  </div>
</template>

<script>

export default {
  name: 'Sidebar',
  data: () => ({
    show: null,
    items: [
      'ПАРКОВА', 'СТРАХОВКА', 'БЕНЗИН', 'ОБСЛУЖИВАНИЕ',
    ],
  }),

};
</script>

<style scoped = "scss">
.nav-btn{
  top: 20px;
  left: 20px;
  color: #ffff;
  cursor: pointer;
  font-size: 50px;
}
li{
  color: white;
  background: #111518;
  list-style-type: none;
}
li:hover{
  cursor: pointer;
  border-color: aqua;
  color: #0EC261;
}
ul{
  position: relative;
  font-family: Roboto;
  font-style: normal;
  font-weight: 500;
  font-size: 32px;
  line-height: 57px;
  z-index: 1;
  width: 100%;
}

</style>
