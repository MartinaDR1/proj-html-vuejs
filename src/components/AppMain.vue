<script>
import SectionSubject from "../components/SectionSubject.vue";
import ContentMain from "../components/ContentMain.vue";
import Blue_Banner from "../components/Blue_Banner.vue";


    export default {
        name:'AppMain',

        components:{
            SectionSubject,
            ContentMain,
            Blue_Banner
        }
    }
</script>

<template>
    <SectionSubject/>
    <ContentMain/>
    <Blue_Banner/>
</template>


<style lang="scss" scoped>
</style>