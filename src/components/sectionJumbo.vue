<script>
export default {
    name: 'sectionJumbo',
    data() {
        return {
            list: [
                {
                    title: 'dc comics',
                    link: [
                        'characters',
                        'comics',
                        'movies',
                        'tv',
                        'games',
                        'videos',
                        'news'
                    ]
                },
                {
                    title: 'dc shop',
                    link: [
                        'shop dc',
                        'shop dc collectibles',
                    ]
                },
                {
                    title: 'dc',
                    link: [
                        'term of use',
                        'privacy policy(new)',
                        'ad choice',
                        'advertising',
                        'jobs',
                        'subscriptions',
                        'talent workshops',
                        'cpsc certificates',
                        'ratings',
                        'shop helps',
                        'contact us'

                    ]
                },
                {
                    title: 'sites',
                    link: [
                        'dc',
                        'mad magazine',
                        'dc kids',
                        'dc universe',
                        'dc power visa'
                    ]
                },
            ]
        }
    }
}
</script>

<template>
    <section class="jumbo">
        <ul v-for="item in list">
            <li>
                <h3 class="text-white text-uppercase mt-5">{{ item.title }}</h3>
                <ul>
                    <li class="text-white" v-for="singleEl in item.link">
                        <a href="">
                            {{ singleEl }}
                        </a>
                    </li>
                </ul>
            </li>
        </ul>
        <div class="dc_logo">

        </div>
    </section>
    <!-- /.jumbo -->
</template>


<style lang="scss" scoped>
.jumbo {
    background-image: url(../assets/img/footer-bg.jpg);
    background-repeat: repeat-x;
    position: relative;
    display: flex;
    flex-direction: column;
    flex-wrap: wrap;




    /* display: flex;
    height: 500px; */
    /* flex-direction: column;
    flex-wrap: wrap;
    align-items: flex-start; */
    height: 500px;

    /* 
    ul {
        display: flex;
        flex-direction: column;
        align-items: flex-start;
    } */




    .dc_logo {
        background-image: url(../assets/img/dc-logo-bg.png);
        background-size: 600px;
        width: 800px;
        aspect-ratio: 1/1;
        background-repeat: no-repeat;
        margin-left: 40rem;
        position: absolute;
        top: -80px
    }
}
</style>