
<script>
import comicList from "./comicList.vue";
export default {
    name: 'sectionContent',
    components: {
        comicList,
    }
}
</script>


<template>
    <section class="jumbo">
        <!-- <img src="../assets/img/jumbotron.jpg" alt=""> -->
    </section>
    <section class="content">
        <comicList />
    </section>
    <!-- /.content -->
</template>

<style lang="scss" scoped>
/* img {
    max-width: 100%;
    width: 100%;
} */
.jumbo {
    background-image: url('../assets/img/jumbotron.jpg');
    height: 400px;
    background-size: cover;
    background-repeat: no-repeat;
}
</style>