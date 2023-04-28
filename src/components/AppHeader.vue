<script>
import Jumbo from "../components/Jumbo.vue";
export default {
    name: 'AppHeader',
    data() {
        return{
            itemNav: [
                {
                    title: "home",
                    link: "#"
                },
                {
                    title: "courses",
                    link: "#"
                },
                {
                    title: "instructors",
                    link: "#"
                },
                {
                    title: "events",
                    link: "#"
                },
                {
                    title: "pages",
                    link: "#"
                },
                {
                    title: "elements",
                    link: "#"
                }
            ]
        }
    },
    components:{
        Jumbo
    }
}
</script>

<template>
    <Jumbo/>
    <nav class="container d-flex justify-content-around py-1">
        <div class="logo py-2">
            <img src="../assets/img/logo-light.png" alt="">
        </div>

        <div class="item d-flex py-3">
            <ul v-for="item in itemNav">
                <li><a href="" class="text-uppercase text-light" >{{ item.title }}</a></li>
            </ul>
        </div>

        <div class="icon py-3 text-light">
            <i class="fa-solid fa-magnifying-glass"></i>
            <i class="fa-solid fa-bag-shopping"></i>
            <i class="fa-solid fa-bars"></i>
        </div>
    </nav>
</template>


<style lang="scss" scoped>
@use '../assets/scss/variables'as *;

img:hover{
    border-bottom: 1px solid yellow;
    border-left-width:medium;
    transition: 3s;
}
nav{
    position: absolute;
    top: 1rem;
    left: 7rem;
    .logo img{
        width: 150px;
    }

    ul{
    list-style: none;

        a{
            text-decoration: none;
            font-size: 12px;
    
        }
    }   
    .icon i{
        padding-right: 1rem;

    }
}

</style>