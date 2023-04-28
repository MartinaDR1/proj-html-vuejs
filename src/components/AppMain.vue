<script>
import SectionSubject from "../components/SectionSubject.vue";
import ContentMain from "../components/ContentMain.vue";
import Blue_Banner from "../components/Blue_Banner.vue";
import Learning from "../components/Learning.vue";
import Courses from "../components/Courses.vue";
import Pricing from "../components/Pricing.vue";
import Partners from "../components/Partners.vue";



    export default {
        name:'AppMain',

        components:{
            SectionSubject,
            ContentMain,
            Blue_Banner,
            Learning,
            Courses,
            Pricing,
            Partners
        }
    }
</script>

<template>
    <SectionSubject/>
    <ContentMain/>
    <Blue_Banner/>
    <Learning/>
    <Courses/>
    <Pricing/>
    <Partners/>
</template>


<style lang="scss" scoped>
</style>