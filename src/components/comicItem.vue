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
    <div class="col mt-5">
        <img :src="thumb" alt="">
        <p class="text-uppercase text-white pt-3">{{ title }}</p>
    </div>

</template>


<style lang="scss" scoped>
p {
    font-weight: 600;
    line-height: 15px;
}

img {
    width: 200px;
    height: 200px;
    object-fit: cover;
}
</style>