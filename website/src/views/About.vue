<template>
  <div class="about">
    <AboutIntro />
    <AboutExperience/>
    <Footer />
  </div>
</template>

<script>
import AboutIntro from "../components/AboutIntro.vue"
import AboutExperience from "../components/AboutExperience.vue"
import Footer from "../components/Footer.vue"

export default{
  name: "About",
  components: {
    AboutIntro,
    AboutExperience,
    Footer
  }
}
</script>


<style>

</style>