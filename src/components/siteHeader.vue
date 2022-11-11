


<script>
export default {
    name: 'siteHeader',
    data() {
        return {
            menu:
                [
                    {
                        name: 'Characters',
                        link: '#'
                    },
                    {
                        name: 'Comics',
                        link: '#'
                    },
                    {
                        name: 'Movies',
                        link: '#'
                    },
                    {
                        name: 'Tv',
                        link: '#'
                    },
                    {
                        name: 'Games',
                        link: '#'
                    },
                    {
                        name: 'Collectibles',
                        link: '#'
                    },
                    {
                        name: 'Videos',
                        link: '#'
                    },
                    {
                        name: 'Fans',
                        link: '#'
                    },
                    {
                        name: 'News',
                        link: '#'
                    },
                    {
                        name: 'Shop',
                        link: '#'
                    },
                ]
        }
    }
}
</script>



<template>
    <header id="site_header">
        <div class="container">
            <div class="d-flex justify-content-between">
                <div class="logo">
                    <img src="../assets/img/dc-logo.png" alt="">
                </div>
                <nav class="nav justify-content-center">
                    <a v-for="item in menu" :href="item.link" class="text-uppercase"
                        :class="item.name === 'Comics' ? 'active' : ''">{{
        item.name
                        }}</a>
                </nav>
            </div>
        </div>
    </header>
</template>


<style lang="scss" scoped>
@use '../assets/scss/partials/variables.scss' as*;

.logo {
    margin-top: 0.5rem;

    img {
        width: 80px;

    }
}

nav {


    a {
        text-decoration: none;
        color: $primary-dark;
        padding-top: 0.7rem;
        padding-left: 0.7rem;
        padding-right: 0.7rem;
        margin-top: 1rem;
        font-weight: 600;

    }

    .active {
        border-bottom: 4px solid $primary;
        color: $primary;
        padding-bottom: 1rem;
    }
}
</style>