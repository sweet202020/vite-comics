<script>
export default {
    name: 'sectionIcon',
    data() {
        return {
            icons: [
                {
                    image: 'comics-digital-comics.png',
                    name: 'Digital comics',
                },
                {
                    image: 'comics-merchandise.png',
                    name: 'Dc merchandise',
                },
                {
                    image: 'comics-subscriptions.png',
                    name: 'Subscription',
                },
                {
                    image: 'comics-shop-locator.png',
                    name: 'comic shop locator',
                },
                {
                    image: 'dc-power-visa.svg',
                    name: 'dc power visa',
                },
            ]
        }
    },
    methods: {
        getImagePath: function (imgPath) {
            return new URL(imgPath, import.meta.url).href
        }
    }
}
</script>

<template>
    <section class="icon">
        <div class="container">
            <div class="row">
                <div class="col" v-for="icon in icons">
                    <div class="my_card">
                        <img :src="getImagePath(`../assets/img/buy-${icon.image}`)" alt="">
                        {{ icon.name }}
                    </div>
                </div>
            </div>
        </div>
    </section>
    <!-- /.icon -->
</template>

<style lang="scss" scoped>
.icon {
    background-color: blue;
    color: white;
    padding: 0 13rem;
}

.my_card {
    padding: 2rem 0;

    img {
        width: 50px;
        height: 50px;
        object-fit: contain;
    }
}
</style>