<script>
export default {
    name: 'Footer'
}
</script>

<template>
    <footer id="site_footer">
        <div class="container">
            <div class="d-flex justify-content-between">
                <button class="text-uppercase">sign-up now</button>
                <div class="icons">
                    <span class="text-uppercase follow">follow us</span>
                    <i class="fa-brands fa-facebook"></i>
                    <i class="fa-brands fa-twitter"></i>
                    <i class="fa-brands fa-youtube"></i>
                    <i class="fa-brands fa-pinterest"></i>
                    <i class="fa-brands fa-periscope"></i>
                </div>

            </div>
        </div>

    </footer>
</template>


<style lang="scss" scoped>
@use '../assets/scss/partials/variables.scss' as*;

footer {
    background-color: $dark-light;
    position: relative;
    z-index: 100;


    button {
        border: 1px solid $primary;
        background-color: transparent;
        color: white;
        padding: 0.75rem 1.5rem;
        margin: 2rem;
    }

    .icons {
        margin: 2rem;

    }

    .follow {
        color: $primary;
        font-weight: 600;
    }

    i {
        background-color: grey;
        border-radius: 50%;
        margin: 0 0.5rem;
        padding: 0.3rem;
    }
}
</style>