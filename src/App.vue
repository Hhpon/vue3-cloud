<template>
  <div id="app">
    <m-header></m-header>
    <tabber></tabber>
    <keep-alive>
      <!-- 使 router-view 的内容缓存到内存中 减轻服务器压力-->
      <router-view></router-view>
    </keep-alive>
    <player></player>
  </div>
</template>

<script>
import MHeader from "components/m-header/m-header";
import Tabber from "components/tabber/tabber";
import Player from "components/player/player";

export default {
  components: {
    MHeader,
    Tabber,
    Player
  }
};
</script>

<style lang="scss">
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
