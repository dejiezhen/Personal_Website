<template>
  <div class="home">
    <IntroHome />
    <HomeProjects />
    <Footer />
  </div>
</template>

<script>
import IntroHome from "../components/IntroHome.vue"
import HomeProjects from "../components/HomeProjects.vue"
import Footer from "../components/Footer.vue"
export default {
  name: 'Home',
  components: {
    IntroHome,
    HomeProjects,
    Footer
  }
}
</script>

<style>
.home{
  display: flex;
  flex-direction: column;
}

</style>
