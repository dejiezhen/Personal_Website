<template>
    <section class="intro-container">
        <header class="intro-quote">
            <p id="intro-p">
                Hello, I'm Dejie.
                <br>
                I Like To Build Stuff
            </p>
        </header>
    </section>
</template>

<script>
export default{
    name: "AboutIntro",
}

</script>

<style lang='scss'>
.intro-container{
    display: flex;
    justify-content: space-between;
    background-image: url("../assets/images/picture_id_final-removebg.png");
    height: 100vh;
    background-repeat: no-repeat;
    background-position: bottom 20% right 15%;
    background-attachment: fixed;
    // background-clip: padding-box;
    background-size: 35rem;
    opacity: .7;
    // border: 1px solid red;
    .intro-quote{
        text-align: left;
        // border:1px solid black;
        padding: 20%;
        #intro-p{
            font-size: 3rem;

        }

    }

}

@media only screen 
  and (min-device-width: 375px) 
  and (max-device-width: 812px) 
  and (-webkit-min-device-pixel-ratio: 3) { 
    .intro-container{
        background-position: top 10rem left 5rem;
        .intro-quote{
            border: 1px solid blue;
        }
        #intro-p{
            padding-top: 50%;
            opacity: 1;
            font-size: .5rem;
            font-weight: 800;
        }
    }
  }

</style>