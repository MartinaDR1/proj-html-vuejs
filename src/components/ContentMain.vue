<script>
export default {
    name: 'ContentMain',


    data() {
        return {
            showButton: false
        };
    },
    methods: {
        scrollToTop() {
            window.scrollTo({
                top: 0,
                behavior: "smooth"
            });
        }
    },
    mounted() {
        window.addEventListener("scroll", () => {
            if (window.pageYOffset > 100) {
                this.showButton = true;
            } else {
                this.showButton = false;
            }
        });
    }

}
</script>

<template>
    <div class="container">
        <h2 class="fw-bolder py-3">The Trusted Name <br> for In-Home Tutoring.</h2>
        <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Possimus earum deserunt ratione quos magni laboriosam
            eligendi aut sapiente tenetur delectus quam pariatur vel molestias beatae, sunt mollitia totam.</p>
        <span><a href="" class="text-uppercase fw-bold text-decoration-none">learn more</a></span>
    </div>

    <div class="banner">
        <img src="../assets/img/h5-img-1.jpg" width="800px" alt="">
        <button @click="scrollToTop" class="scroll"><i class="fa-solid fa-angle-up"></i></button>
    </div>


    <div class="empowering container py-5 d-flex">
        <div class="row">
            <div class="col-7">
                <div class="img py-5 text-center">
                    <img src="../assets/img/h5-img-2.jpg" width="500px" alt="">
                </div>
            </div>


            <div class="col-5">

                <div class="text">
                    <h2 class="fw-bold">Empowering <br> Children to Reach <br> Their Potential.</h2>
                    <p class="py-5">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Perferendis dolorum qui
                        necessitatibus nobis optio labore, hic veniam totam saepe voluptate, eaque harum nulla consequuntur
                        iste quibusdam!</p>

                    <div class="num d-flex">
                        <div class="left">
                            <h2 class="fw-bold">168</h2>
                            <h3>User Stories</h3>
                        </div>
                        <div class="right px-5">
                            <h2 class="fw-bold">347</h2>
                            <h3>Events</h3>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>


<style lang="scss" scoped>
@use '../assets/scss/variables' as *;

a,
.left,
.right {
    color: $txt-blue_light;
}

.banner {
    text-align: center;
    position: relative;
}

.scroll{
    background-color: $bg-blue;
    border: 0;
    position: absolute;
    right: 0;
    top: 5rem;
}


</style>