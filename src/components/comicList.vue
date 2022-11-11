<script>
import dcComics from "../data/dcComics.js";
export default {
    name: 'comicList',
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
            <div class="col" v-for="comic in comics">
                <img :src="comic.thumb" alt="">
                <p>{{ comic.series }}</p>
            </div>

        </div>
    </div>

</template>