<template>

    <div class="word-carousel">
        <h1>Dejie Zhen</h1>
        <span>Software Developer</span>
    </div>

</template>

<script>
export default{
    name: "IntroHome",
}
</script>

<style scoped lang="scss">
.word-carousel{
    font-weight: bold;
    display: flex;
    align-items: left;
    justify-content: left;
    flex-direction: column;
    text-align: left;
    margin-top: 10rem;
    margin-left: 5rem;
    padding: 3rem;
}
.word-carousel h1 {
    font-size: 7rem;
}
.word-carousel span{
    padding-left: .5rem;
}

@media only screen 
  and (min-device-width: 375px) 
  and (max-device-width: 812px) 
  and (-webkit-min-device-pixel-ratio: 3) { 
      .word-carousel {
          margin: 10rem auto;
      }

  }


</style>

