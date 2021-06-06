<template>
  <div id="app">
    <Navbar />
    <transition name="router-anim" enter-active-class="animated shakeX" leave-active-class="animated slideOutRight">
      <router-view/>
    </transition>
  </div>
</template>

<script>
import Navbar from './components/Navbar.vue'
export default{
  name: "App",
  components: {
    Navbar
  }
}

</script>

<style lang="scss">
@import "https://cdn.jsdelivr.net/npm/animate.css@3.5.1";
*{
  padding: 0;
  margin: 0;
  box-sizing: border-box;

}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  overflow-x: hidden;
}

</style>
