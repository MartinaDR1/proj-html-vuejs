<script>
    export default {
        name: 'Jumbo'
        
    }
</script>

<template>
<div class="jumbo">
    <div class="sm_container text">
        <h1 class="p-3 fw-bold text-light">Contemporary Ideas</h1>
        <p class="px-5">Lorem Ipsn gravida nibh vel velit auctor aliquetnean sollicitudin, lorem quis bibendum auci elit consequat ipsutis sem nibh id elited odio sit amet nibcursus a sit amet mauris.</p>
        
        <button type="submit" class="text-uppercase text-light fw-semibold border-0 my-4">register now</button>
    </div>
</div>
</template>


<style lang="scss" scoped>
@use '../assets/scss/variables'as *;

    .sm_container{
        margin: auto;
        width: 70%;
    }
    .jumbo{
        background-image: url(../assets/img/h5-slide-3-background.jpg);
        background-position: bottom;
        height: 600px;

        .text{
            padding-top: 10rem;
            text-align: center;
            
            p{
                color: $txt-dark_light
            }

            button{
                background-color: $bg-blue;
                padding: 0.75rem 2rem;
                font-size: 12px;
            }
        }   
    }

</style>