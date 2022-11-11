<script>
export default {
    name: 'sectionJumbo',


}
</script>

<template>
    <section class="jumbo">
        <div class="container">
            <div class="d-flex">

                <ul>
                    <li>
                        <h3 class="text-white text-uppercase mt-5">dc comics</h3>
                        <ul>
                            <li class="text-white"><a href="">Characters</a></li>
                            <li class="text-white"><a href="">Comics</a></li>
                            <li class="text-white"><a href="">Movies</a></li>
                            <li class="text-white"><a href="">TV</a></li>
                            <li class="text-white"><a href="">Games</a></li>
                            <li class="text-white"><a href="">Videos</a></li>
                            <li class="text-white"><a href="">News</a></li>
                            <li>
                                <ul>
                                    <li>
                                        <h3 class="text-white text-uppercase mt-5">shop</h3>
                                        <ul>
                                            <li class="text-white"><a href="">Shop DC</a></li>
                                            <li class="text-white"><a href="">Shop DC Collectibles</a></li>
                                        </ul>
                                    </li>
                                </ul>

                            </li>
                        </ul>
                    </li>
                </ul>
                <ul>
                    <li>
                        <h3 class="text-white text-uppercase mt-5">dc</h3>
                        <ul>
                            <li class="text-white"><a href="">Term of Use</a></li>
                            <li class="text-white"><a href="">Privacy Policy (new)</a></li>
                            <li class="text-white"><a href="">Ad choice</a></li>
                            <li class="text-white"><a href="">Advertising</a></li>
                            <li class="text-white"><a href="">Jobs</a></li>
                            <li class="text-white"><a href="">Subscriptions</a></li>
                            <li class="text-white"><a href="">Talent Workshops</a></li>
                            <li class="text-white"><a href="">CPSCS Certificates</a></li>
                            <li class="text-white"><a href="">Ratings</a></li>
                            <li class="text-white"><a href="">Shop help</a></li>
                            <li class="text-white"><a href="">Contact Us</a></li>
                        </ul>
                    </li>
                </ul>
                <ul>
                    <li>
                        <h3 class="text-white text-uppercase mt-5">sites</h3>
                        <ul>
                            <li class="text-white"><a href="">DC</a></li>
                            <li class="text-white"><a href="">MAD Magazine</a></li>
                            <li class="text-white"><a href="">DC kids</a></li>
                            <li class="text-white"><a href="">DC Universe</a></li>
                            <li class="text-white"><a href="">DC Power Visa</a></li>
                        </ul>
                    </li>
                </ul>
            </div>

        </div>
        <div class="dc_logo">

        </div>
    </section>
    <!-- /.jumbo -->
</template>


<style lang="scss" scoped>
@use '../assets/scss/partials/variables.scss' as*;

.jumbo {
    background-image: url(../assets/img/footer-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover;
    position: relative;
    display: flex;
    flex-direction: column;
    flex-wrap: wrap;


    ul {
        list-style: none;
        padding-left: 0;
        margin-right: 1rem;
        padding-bottom: 1rem;

        h3 {
            font-weight: bold;
        }

        a {
            text-decoration: none;
            color: gray;
            font-weight: 600;
        }
    }



    .dc_logo {
        background-image: url(../assets/img/dc-logo-bg.png);
        background-size: 600px;
        width: 800px;
        aspect-ratio: 1/1;
        background-repeat: no-repeat;
        right: 0;
        position: absolute;
        top: -80px
    }
}
</style>