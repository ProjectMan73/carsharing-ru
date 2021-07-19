<template>
<div class="the-header">
<p>Need for drive</p>
  <v-icon id="map__icon">mdi-map-marker-outline</v-icon>
  <p1 id="location">Ульяновск</p1>
  <div class="main-label">
    <h1>Каршеринг</h1>
    <h2>Need for drive</h2>
    <h3>Поминутная аренда авто твоего города</h3>
    <v-btn elevation="2" id="btn__book">Забронировать</v-btn>
  </div>
</div>
</template>

<script>
export default {
  name: 'TheHeader',
};
</script>

<style scoped="scss">
p{
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
#map__icon{
  position: absolute;
  position: absolute;
  width: 103px;
  height: 16px;
  left: 565px;
  top: 44px;
  color: #999999;

}
#location{
  position: absolute;
  position: absolute;
  width: 103px;
  height: 16px;
  left: 630px;
  color: #999999;
  top: 44px;
  font-family: Roboto;
  font-style: normal;
  font-weight: normal;
  font-size: 14px;
  line-height: 16px;
}
h1{
  position: absolute;
  width: 367px;
  height: 66px;
  left: 128px;
  top: 227px;

  font-family: Roboto;
  font-style: normal;
  font-weight: bold;
  font-size: 70px;
  line-height: 66px;

  /* identical to box height */

  /* Black */
  color: #121212;
}
h2{
  position: absolute;
  width: 447px;
  height: 66px;
  left: 128px;
  top: 297px;

  font-family: Roboto;
  font-style: normal;
  font-weight: bold;
  font-size: 70px;
  line-height: 66px;

  /* identical to box height */

  /* Main accent */
  color: #0EC261;
}
h3{
  position: absolute;
  width: 560px;
  height: 30px;
  left: 128px;
  top: 397px;

  font-family: Roboto;
  font-style: normal;
  font-weight: 300;
  font-size: 26px;
  line-height: 30px;

  /* Gray */
  color: #999999;
}
#btn__book{
  position: absolute;
  width: 250px;
  height: 48px;
  left: 128px;
  top: 497px;

  font-family: Roboto;
  font-style: normal;
  font-weight: 300;
  font-size: 16px;
  line-height: 30px;

  /* Gray */
  color: white;
  background: linear-gradient(90deg, #0EC261 2.61%, #039F67 112.6%);
  background-blend-mode: darken;
  border-radius: 8px;
}
</style>
