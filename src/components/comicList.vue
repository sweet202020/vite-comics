<script>
import dcComics from "../data/dcComics.js";
import comicItem from "./comicItem.vue";
export default {
    name: 'comicList',
    components: {
        comicItem
    },
    data() {
        return {
            comics: dcComics
        }
    }
}
</script>

<template>


    <div class="container">
        <div class="row row-cols-2 row-cols-sm-4 row-cols-md-6">
            <comicItem v-for="comic in comics" :thumb="comic.thumb" :title="comic.series" />
        </div>
    </div>

</template>