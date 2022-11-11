
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
        <div class="container">
            <h3 class="text-uppercase">current series</h3>
            <comicList />
            <div class="text-center">
                <button class="text-uppercase">load more</button>
            </div>
        </div>
    </section>
    <!-- /.content -->
</template>




<style lang="scss" scoped>
@use '../assets/scss/partials/variables.scss' as*;


.jumbo {
    background-image: url('../assets/img/jumbotron.jpg');
    height: 400px;
    background-size: cover;
    background-repeat: no-repeat;
}

.content {
    background-color: $primary-dark;

    h3 {
        margin-top: -1rem;
    }

    button,
    h3 {
        background-color: $primary;
        font-weight: 600;
        color: $lighter;
        padding: 0.5rem 2rem;
        margin-bottom: 1rem;
        display: inline-block;
    }
}
</style>