<template>
<div class="menu-burger">
    <v-icon class="nav__btn" v-if="!show" @click="show = !show" key="menu">mdi-menu</v-icon>
    <v-icon class="nav__btn" v-else @click="show = !show" key="close">mdi-close</v-icon>
  <transition name="fade">
    <ul v-if="show">
      <li v-for="item in items" v-bind:key="item">{{item}}</li>
    </ul>
  </transition>
</div>
</template>

<script>
export default {
  name: 'Menuburger',
  data() {
    return {
      items: [
        'ПАРКОВА', 'СТРАХОВКА', 'БЕНЗИН', 'ОБСЛУЖИВАНИЕ',
      ],
      show: false,
    };
  },
};
</script>

<style scoped="scss">
.nav__btn{
  top: 20px;
  left: 20px;
  color: white;
  cursor: pointer;
  font-size: 3em;
  transition: all .3s ease;
  transform: translateX(-100%);
}
li{
  align-items: center;
  color: black;
  cursor: pointer;
  display: flex;
  justify-content: center;
  list-style-type: none;
  text-transform: uppercase;
  background-color: rosybrown;
  transition: .5s;
}
li:hover{
  border-color: aqua;
  color: red;
}

</style>
