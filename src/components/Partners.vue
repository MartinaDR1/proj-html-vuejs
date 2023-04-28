<script>
    export default {
        name:'Partners',

        data(){
            return{
                partner:[
                '../../public/h5-client-5-h.png',
                '../../public/h5-client-2-h.png',
                '../../public/h5-client-4-h.png',
                '../../public/h5-client-1-h.png',
                ]
            }
        }

    }
</script>

<template>
    <div class="container py-5">
        <img :src="logo" alt="" v-for="logo in partner">
    </div>
</template>


<style lang="scss" scoped></style>