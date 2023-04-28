<script>
export default {
    name: 'Courses',

    data() {
        return {
            cards: [
                {
                    id: 1,
                    image: '../../public/course-5-f-img.jpg',
                    title: "Android Developer",
                    name: 'David Sanders',
                    price: 'free',
                    text: 'Lorem ipsum dolor sit amet consectetur, adipisicing elit. Suscipit numquam eos ducimus reprehenderit odit rem, sequi ad sapiente.',
                    icon: '1',
                    sub: 'programming'

                },
                {
                    id: 2,
                    image: '../../public/course-6-f-img.jpg',
                    title: "Web Designing",
                    name: 'Jennifer Powell',
                    price: 'free',
                    text: 'Lorem ipsum dolor sit amet consectetur, adipisicing elit. Suscipit numquam eos ducimus reprehenderit odit rem, sequi ad sapiente.',
                    icon: '1',
                    sub: 'programming'
                },
                {
                    id: 3,
                    image: '../../public/course-12-f-img.jpg',
                    title: "Financial Modeling",
                    name: 'Edward Bowman',
                    price: '$20',
                    text: 'Lorem ipsum dolor sit amet consectetur, adipisicing elit. Suscipit numquam eos ducimus reprehenderit odit rem, sequi ad sapiente.',
                    icon: '1',
                    sub: 'business'
                },/*
                {
                    id: 4,
                    image: '../../public/h5-custom-icon-1.png',
                    title: "Business Englsh",
                    name: 'Prestan Marshall',
                    price: '$20',
                    text: 'Lorem ipsum dolor sit amet consectetur, adipisicing elit. Suscipit numquam eos ducimus reprehenderit odit rem, sequi ad sapiente.',
                    icon: '1',
                    sub: 'Languages'
                },
                {
                    id: 5,
                    image: '../../public/h5-custom-icon-1.png',
                    title: "Social Computing",
                    name: 'David Sanders',
                    price: 'free',
                    text: 'Lorem ipsum dolor sit amet consectetur, adipisicing elit. Suscipit numquam eos ducimus reprehenderit odit rem, sequi ad sapiente.',
                    icon: '1',
                    sub: 'Programming'
                },
                {
                    id: 6,
                    image: '../../public/h5-custom-icon-1.png',
                    title: "Basic Marketing",
                    name: 'Edward Bowman',
                    price: '$43',
                    text: 'Lorem ipsum dolor sit amet consectetur, adipisicing elit. Suscipit numquam eos ducimus reprehenderit odit rem, sequi ad sapiente.',
                    icon: '1',
                    sub: 'business'
                },
                {
                    id: 7,
                    image: '../../public/h5-custom-icon-1.png',
                    title: "Android Developer",
                    name: 'David Sanders',
                    price: 'free',
                    text: 'Lorem ipsum dolor sit amet consectetur, adipisicing elit. Suscipit numquam eos ducimus reprehenderit odit rem, sequi ad sapiente.',
                    icon: '1',
                    sub: 'programming'

                },
                {
                    id: 8,
                    image: '../../public/h5-custom-icon-1.png',
                    title: "Web Designing",
                    name: 'Jennifer Powell',
                    price: 'free',
                    text: 'Lorem ipsum dolor sit amet consectetur, adipisicing elit. Suscipit numquam eos ducimus reprehenderit odit rem, sequi ad sapiente.',
                    icon: '1',
                    sub: 'programming'
                },
                {
                    id: 9,
                    image: '../../public/h5-custom-icon-1.png',
                    title: "Financial Modeling",
                    name: 'Edward Bowman',
                    price: '$20',
                    text: 'Lorem ipsum dolor sit amet consectetur, adipisicing elit. Suscipit numquam eos ducimus reprehenderit odit rem, sequi ad sapiente.',
                    icon: '1',
                    sub: 'business'
                }*/
            ],

        }
    }

}
</script>


<template>
    <div class="courses">
        <div class="text text-center container">
            <h2>Popular Online Courses</h2>
            <p class="px-5">Lorem ipsum dolor sit amet consectetur adipisicing elit. Expedita, facilis illum voluptatum
                asperiores consequuntur ab nam dolor deserunt suscipit sequi.
            </p>
        </div>

        <div class="container d-flex">
            <div class="card border" v-for="course in cards" :key="cardIndex">
                <img  :src="course.image" alt="">

                <div class="header d-flex justify-content-between p-2">
                    <div class="info">
                        <h6 class="fw-bold">{{ course.title }}</h6>
                        <span class="fw-semibold">{{ course.name }}</span>
                    </div>

                    <div class="price">
                        <span class="badge rounded-pill text-bg-warning text-uppercase text-light" v-if="course.price === 'free'">{{ course.price }}</span>
                        <span class="badge rounded-pill text-bg-primary text-uppercase text-light px-3" v-else>{{ course.price }}</span>
                    </div>
                </div>

                <div class="body px-2">
                    <p >{{ course.text }}</p>
                </div>

                <div class="footer d-flex px-2">
                    <div class="icon p-1 ">
                        <i class="fa-solid fa-user fa-xs"></i>
                        <span class="fw-semibold px-2">{{ course.icon }}</span>
                    </div>

                    <div class="sub p-1 ">
                        <i class="fa-solid fa-tag fa-rotate-90 fa-xs"></i>
                        <span class="text-uppercase fw-semibold px-2">{{ course.sub }}</span>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>


<style lang="scss" scoped>
@use '../assets/scss/variables' as *;

.courses {
    background-image: url(../assets/img/page-background-img.png);
    max-height: 600px;
    padding: 1rem 0;
    border-top: 1px solid  $txt-dark_light;
    border-bottom: 1px solid  $txt-dark_light;

    .card {
        width: calc(100% / 3 - 1rem);
        margin: 1rem;
    }

    .footer,
    span{
        color: $txt-dark_light;
    }
}
</style>