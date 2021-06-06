<template>
    <div class="container">
        <img :src="picture" :alt="alt_picture" class="image" id="project">
        <div class="middle">
            <div class="text">{{text}}</div>
        </div> 
    </div>

</template>

<script>
export default{
    name: "Projects",
    props: {
        picture: String,
        text: String,
        alt_picture: String,
        id: String,
    },
}

</script>

<style lang="scss">
.container{
    padding: 1rem;
    position: relative;
    .image {
        position: absolute;
        left: 0;
        top: 0;
        max-width: 100%;
        margin: auto;
        bottom: 0;
        right: 0;
        width: 100%;
        opacity: 1;
        display: block;
        transition: .5s ease;
        backface-visibility: hidden;
    }
    .middle{
        transition: .5s ease;
        opacity: 0;
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        -ms-transform: translate(-50%, -50%);
        text-align: center;
        .text{
            color: white;
            font-size: 16px;
            padding: 16px 32px;
            background-color: gray;
            border-radius: 15px;
        }
    }

}

.container:hover .image{
    opacity: 0.3;
}
.container:hover .middle{
    opacity: 1;
}
.container::before{
    content: "";
    padding-top: 100%;
    display: block;

}

</style>