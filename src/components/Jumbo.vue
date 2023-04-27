<script>
export default {
    name: 'Jumbo',

    data() {
        return {
            activeImage: 0,
            slider: [
                '../../public/h5-slide-1-background.jpg',
                '../../public/h5-slide-2-background.jpg',
                '../../public/h5-slide-3-background.jpg',
            ],
        }
    },
    computed: {
        currentImage() {
            return this.slider[this.activeImage]
        }
    },
    mounted() {
        setInterval(() => {
            this.activeImage++
            if (this.activeImage === this.slider.length) {
                this.activeImage = 0

            }

        }, 2000)
    }

}
</script>

<template>
    <div class="jumbo">

        <img :src="currentImage" alt="">

        <div class="sm_container text">
            <h1 class="p-3 fw-bold text-light">Contemporary Ideas</h1>
            <p class="px-5">Lorem Ipsn gravida nibh vel velit auctor aliquetnean sollicitudin, lorem quis bibendum auci elit
                consequat ipsutis sem nibh id elited odio sit amet nibcursus a sit amet mauris.</p>

            <button type="submit" class="text-uppercase text-light fw-semibold border-0 my-4">register now</button>
        </div>

        <div class="carousel-indicators">
          <button class="border-0 bg-transparent" v-for="(image, index) in slider" :key="index" :class="{ active: activeImage === index }"><i class="fa-solid fa-circle"></i></button>
        </div>
    </div>
</template>


<style lang="scss" scoped>
@use '../assets/scss/variables' as *;

.sm_container {
    margin: auto;
    width: 70%;
}

.jumbo {
    img {
        width: 100%;
        position: relative;
    }

    .text {
        padding-top: 10rem;
        text-align: center;
        position: absolute;
        top: 5rem;
        left: 12rem;

        p {
            color: $txt-dark_light
        }

        button {
            background-color: $bg-blue;
            padding: 0.75rem 2rem;
            font-size: 12px;
        }
    }

    button.active {
  color: white;
}
}
</style>

