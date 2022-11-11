<script>
export default {
    name: 'comicItem',
    props: {
        thumb: String,
        title: String
    }
}
</script>

<template>
    <div class="col">
        <img :src="thumb" alt="">
        <p>{{ title }}</p>
    </div>

</template>