<template>
    <section class="projects-container">
        <h1>Projects</h1>
        <div class="grid">
            <div :key="project.id" v-for="project in projects" class="grid-inner">
                <Projects 
                    :picture = "project.picture"
                    :alt_picture = "project.alt_picture"
                    :text = "project.text"
                    :id = "project.id"
                />
            </div>
        </div>

    </section>
</template>

<script>
import Projects from "./Projects.vue"
export default{
    name: "HomeProjects",
    components:{
        Projects
    },
    data(){
        return {
            projects: []
        }
    },
    created(){
        this.projects = [
            {
                id: "meltea",
                picture: require('../assets/images/logo_transparent.png'),
                alt_picture: "Mel Tea Project",
                text: "Mel Tea" 
            },
            {
                id: "Chatbox",
                picture: require('../assets/images/logo_transparent.png'),
                alt_picture: "Chatbox Project",
                text: "Chatbox" 
            },
            {
                id: "Webscrape",
                picture: require('../assets/images/logo_transparent.png'),
                alt_picture: "Webscraping Project",
                text: "Web Scraper" 
            },
            {
                id: "Webscrape2",
                picture: require('../assets/images/logo_transparent.png'),
                alt_picture: "Webscraping Project",
                text: "Web Scraper" 
            },
            {
                id: "Webscrape3",
                picture: require('../assets/images/logo_transparent.png'),
                alt_picture: "Webscraping Project",
                text: "Web Scraper" 
            },
            {
                id: "Webscrape4",
                picture: require('../assets/images/logo_transparent.png'),
                alt_picture: "Webscraping Project",
                text: "Web Scraper" 
            }

        ]
    }


}
</script>

<style lang="scss">
.projects-container{
    width: 75%;
    margin: 0 auto;
    display: flex;
    padding-top: 10rem;
    height: 50rem;
    flex-direction: column;
    text-align: center;
    height: auto;
    .grid{
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(380px,1fr));
        grid-template-rows: repeat(auto-fill, minmax(380px,1fr));
        gap: 1rem;
        overflow-x: hidden;
    }
}

</style>