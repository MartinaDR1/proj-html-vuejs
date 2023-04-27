<script>
    export default {
        name: 'SectionSubject',

        data(){
            return{
                subject: [
                    {
                        title: "Languages",
                        image: '../../public/h5-custom-icon-1.png'
                    },
                    {
                        title: "Software",
                        image: '../../public/h5-custom-icon-2.png'
                    },
                    {
                        title: "Business",
                        image: '../../public/h5-custom-icon-3.png'
                    },
                    {
                        title: "Chemistry",
                        image: '../../public/h5-custom-icon-4.png'
                    },
                    {
                        title: "Science",
                        image: '../../public/h5-custom-icon-5.png'
                    },
                    {
                        title: "DIY&Craft",
                        image: '../../public/h5-custom-icon-6.png'
                    }
                ]
            }
        }
    }
</script>

<template>
      <div class="container my-5">
        <div class="row">
            <div class="box border py-4 " v-for="sub in subject">
                <img class="py-3" :src="sub.image" alt="">
                <h6 class="py-4 fw-bold">{{ sub.title }}</h6>
            </div>
        </div>
    </div>
</template>


<style lang="scss" scoped>
@use '../assets/scss/variables' as *;

.box{
    width: (100% / 7 );
    background-color: $bg-light_blue;
    margin-right: 1.5rem;
    text-align: center;
}
</style>