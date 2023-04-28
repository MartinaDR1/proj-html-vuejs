<script>
export default {
    name: 'FooterBottom',

    data(){
        return{
            bottom: this.text[0],
        }
    },
    props: [
        'text'
    ],
}

</script>

<template>
    <hr>
    <div class="container d-flex justify-content-between grey-light pb-5">
        <div class="left">
            <span v-for="item in text[0] ">
                {{ item }}
            </span>
        </div>
        <div class="right">
            <span v-for="item in text[1]">
                {{ item }}
            </span>
            <span v-for="item in text[2]" >
                {{ item }}
            </span>
            
            <a href=""><i class="fa-brands fa-twitter px-3" ></i></a>
            <a href=""><i class="fa-brands fa-instagram px-3" ></i></a>
            <a href=""><i class="fa-brands fa-facebook px-3" ></i></a>
        </div>
    </div>
</template>


<style lang="scss" scoped>
@use '../assets/scss/variables' as *;

    hr{
        color: $txt-dark-light;
        width: 70%;
        margin: auto;
        padding: 1rem 0;
    }

    i{
        color:$txt-dark-light ;
    }
</style>