<script>
export default {
    name: 'Blue_Banner',

    data() {
        return {
            activeReview: 0,
            reviews: [
                {
                    image: '../../public/instructor-img-6-150x150.jpg',
                    text: "Mroin gravida nibh vel valiauctor aliquenean sollicitudin, lorem quis bibendum auctor, nisi alit consequat ipsutis sem nibh id elit. Duis sed odio sit amet nivulputate cursus a sit amet mauris. Morbi accumsan ipsum velit. Nam nec tellus",
                    name: 'Joan Collins',
                    job: 'student'
                },
                {
                    image: '../../public/instructor-img-8-150x150.jpg',
                    text: "Lorem ipsum, dolor sit amet consectetur adipisicing elit. Dignissimos dolorum laborum consectetur totam maiores natus commodi labore voluptas error quos.",
                    name: 'Megan White',
                    job: 'student'
                },
                {
                    image: '../../public/instructor-img-1-150x150.jpg',
                    text: "Lorem ipsum, dolor sit amet consectetur adipisicing elit. Lorem ipsum, dolor sit amet consectetur adipisicing elit",
                    name: 'Ed Collins',
                    job: 'student'
                },
                {
                    image: '../../public/instructor-img-4-150x150.jpg',
                    text: "Mroin gravida nibh vel valiauctor aliquenean sollicitudin, lorem quis bibendum auctor, nisi alit consequat ipsutis sem nibh id elit. ",
                    name: 'Syd Red',
                    job: 'student'
                },
                {
                    image: '../../public/instructor-img-9-150x150.jpg',
                    text: "Mroin gravida nibh vel valiauctor aliquenean sollicitudin, lorem quis bibendum auctor, nisi alit consequat ipsutis sem nibh id elit. Duis sed odio sit amet nivulputate cursus a sit amet mauris. Morbi accumsan ipsum velit. Nam nec tellus",
                    name: 'Joan Collins',
                    job: 'student'
                }
            ]
        }
    },
    mounted() {
        setInterval(() => {
            this.activeReview++
            if (this.activeReview === this.reviews.length) {
                this.activeReview = 0
            }

        }, 4000)
    }
}
</script>
<template>
    <div class="banner py-5">
        <div class="container text-center text-light">
            <img class="py-3 rounded-circle" :src="reviews[activeReview].image" alt="">
            
            <div class="text p-5">
                <p class="px-5">{{ reviews[activeReview].text }}</p>
                <h5 class="py-4 fw-bold">{{ reviews[activeReview].name }}</h5>
                <span class="text-uppercase fw-semibold">{{ reviews[activeReview].job }}</span>
            </div>

            <div class="pb-2">
                <button class="border-0 bg-transparent" v-for="(image, index) in reviews" :key="index" :class="{ active: activeReview === index }"><i class="fa-solid fa-circle fa-2xs"></i></button>
            </div>
        </div>
    </div>
</template>


<style lang="scss" scoped>
@use '../assets/scss/variables' as *;

.banner {
    background-image: url(../assets/img/h5-parallax-img-1.png);
    max-height: 550px;

    button:not(.active){
        color: $txt-blue_light
    }
    button.active {
        color: white;
    }
}
</style>