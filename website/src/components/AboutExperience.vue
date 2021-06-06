<template>
    <main class="main-intro">
        <section class="section-left">
            <p>
                Once upon a time, I wanted to be a neurosurgeon, but I quickly changed my mind
                when I wrote my first line of code in python
            </p>
            <br>
            <p>
                I always had a knack for building things and when I started to building projects
                with code, I immediately fell in love.
            </p>
            <br>
            <p>

            </p>
        </section>
        <section class="section-right">
            <div class="experience">
                <h1 class="intro-h1">Experience</h1>
                <p class="details">Unum</p> 
                <span class="detail-date">(6/2021-8/2021)</span>

                <p class="details">Dreams For School</p>
                <span class="detail-date">(6/2021-8/2021)</span>   

                <p class="details">Cedars-Sinai Accelerator</p>
                <span class="detail-date">(6/2021-8/2021)</span>

                <p class="details">Zilkha Neurogenetic Institute</p>
                <span class="detail-date">(6/2021-8/2021)</span>
            </div>
            <div class="education">
                <h1 class="intro-h1">Education</h1>
                <p class="details">Bowdoin College</p>
                <span class="detail-date">(6/2021-8/2021)</span>

                <p class="details">East Los Angeles College</p>
                <span class="detail-date">(6/2021-8/2021)</span>

                <p class="details">Downtown Magnets High School</p>
                <span class="detail-date">(6/2021-8/2021)</span>

            </div>
            <div>
                <h1 class="intro-h1">Tools</h1>
                <div class="programming-lang-grid">
                    <!-- Probably put this into component? -->
                    <div><img class="lang-logo" src="../assets/images/768px-Python-logo-notext.svg.png" alt="Python Logo"></div>
                    <div><img class="lang-logo" src="../assets/images/Java-Logo.png" alt="Java Logo"></div>
                    <div><img class="lang-logo" src="../assets/images/html5-10-569380.png" alt="HTML Logo"></div>
                    <div><img class="lang-logo" src="../assets/images/CSS3_logo_and_wordmark.svg.png" alt="CSS Logo"></div>
                    <div><img class="lang-logo" src="../assets/images/jscript.png" alt="Javascript Logo"></div>
                    <div><img class="lang-logo" src="../assets/images/Vue.js_Logo_2.svg.png" alt="Vuejs Logo"></div>
                    <div><img class="lang-logo" src="../assets/images/Git-Icon-1788C.png" alt="Git Logo"></div>
                    <div><img class="lang-logo" src="../assets/images/c-programming-569564.webp" alt="C Logo"></div>
                </div>
            </div>
        </section>
    </main>
</template>

<script>
export default{
    name:"AboutExperience"
}
</script>

<style scoped lang="scss">
.main-intro{    
    display: flex;
    // justify-content: space-between ;
    width: 75%;
    margin: 0 auto;
    .section-left{
        width: 100%;
        flex-grow: 1;
        padding: 4rem;
        font-size: 2rem;
    }
    .section-right{
        flex-grow: 1;
        width: 100%;
        padding: 4rem;
        .experience, .education{
            margin-bottom: 3rem;
    
        }
        .programming-lang-grid{
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(125px, 1fr));
            grid-template-rows: repeat(auto-fill, minmax(125px, 1fr));
            gap: .5rem;
            place-items: center;
            position: relative;
        }
        .lang-logo{ 
            width: 25%;
        }
          
    }
    .intro-h1{
        font-size: 1.7rem;
    }
    .details{
        font-size: 1rem;
        font-weight: 800;
        display: inline-block;
    }
    .detail-date{
        margin-bottom: .5rem;
        display:block;
    }
}

  
/* Portrait and Landscape */
@media only screen 
  and (min-device-width: 375px) 
  and (max-device-width: 812px) 
  and (-webkit-min-device-pixel-ratio: 3) { 
    .main-intro{
        flex-direction: column;
    }
    .section-left > p{
        font-size: 1.3rem;
    }

}


</style>
