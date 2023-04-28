<script>
export default {
    name: 'FooterTop',

    data(){
        return{
            list1: this.list[0],
            popular: this.list[1],
            support: this.list[2]
        }
    },
    props: [
        'list'
    ],
}
</script>

<template>
    <div class="container d-flex justify-content-between py-5">

        <ul class="text-light ">
            <img src="../assets/img/footer-logo-1.png" width="150" class="py-4">

            <li v-for="item in list1"><a href="" >{{ item.text }}</a></li>
        </ul>
    
        <ul class="text-light">
            <h6  class="py-4">Popular Courses</h6>
            <li v-for="item in popular" class="py-2 fw-semibold">
                <a href="">{{ item.text }}</a>
                <span class="fw-light d-block">{{ item.name }}</span>
            </li>
        </ul>
    
        <ul class="text-light">
            <h6  class="py-4">Support</h6>
            <li v-for="item in support"><a href="">{{ item.text }}</a></li>
        </ul>

        <ul class="text-light">
            <h6  class="py-4">Flexible Learning</h6>
            <img src="../assets/img/footer-img-1.png"  width='300' alt="">
        </ul>
    </div>
</template>


<style lang="scss" scoped>
@use '../assets/scss/variables' as *;

ul{
    list-style: none;

    a{
        text-decoration: none;
        color: $txt-dark-light;
    }
}
</style>