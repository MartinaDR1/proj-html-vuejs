<template>
    <div>
        <button @click="scrollToTop" class="scroll"><i class="fa-solid fa-angle-up"></i></button>
    </div>
</template>

<script>
    export default {
        name: 'Button',

        methods: {
        scrollToTop() {
            window.scrollTo({
                top: 0,
                behavior: "smooth"
            });
        }
    }
    }
</script>

<style lang="scss" scoped>
@use '../assets/scss/variables' as *;

.scroll{
    background-color: $bg-blue;
    border: 0;
    position: absolute;
    right: 0;
}

</style>