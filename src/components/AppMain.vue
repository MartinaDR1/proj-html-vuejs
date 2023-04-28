<script>
import SectionSubject from "../components/SectionSubject.vue";
import ContentMain from "../components/ContentMain.vue";
import Blue_Banner from "../components/Blue_Banner.vue";
import Learning from "../components/Learning.vue";
import Courses from "../components/Courses.vue";


    export default {
        name:'AppMain',

        components:{
            SectionSubject,
            ContentMain,
            Blue_Banner,
            Learning,
            Courses
        }
    }
</script>

<template>
    <SectionSubject/>
    <ContentMain/>
    <Blue_Banner/>
    <Learning/>
    <Courses/>
</template>


<style lang="scss" scoped>
</style>