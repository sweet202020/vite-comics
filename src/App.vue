<script>
export default {
  name: 'App'
}

</script>


<template>
  <header id="site_header">
    <div class="d-flex">
      <div class="logo">
        <img src="./assets/img/dc-logo.png" alt="">
      </div>
      <nav class="nav justify-content-center  ">
        <a class="nav-link active" href="#" aria-current="page">Active link</a>
        <a class="nav-link" href="#">Link</a>
        <a class="nav-link disabled" href="#">Disabled link</a>
      </nav>

    </div>
  </header>
  <!-- /#site_header -->
  <main id="site_main"></main>
  <!-- /#site_main -->
  <footer id="site_footer"></footer>
  <!-- /#site_footer -->

</template>


<style lang="scss">
nav {
  background-color: red;

  a {
    text-decoration: none;
    color: white;
  }
}
</style>