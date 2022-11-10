<script>
import siteHeader from "./components/siteHeader.vue";
import sectionContent from "./components/sectionContent.vue";
import sectionIcon from "./components/sectionIcon.vue";
import sectionJumbo from "./components/sectionJumbo.vue";
export default {
  name: 'App',
  components: {
    siteHeader,
    sectionContent,
    sectionIcon,
    sectionJumbo,
  }
}

</script>


<template>
  <siteHeader />
  <!-- /#site_header -->
  <main id="site_main">
    <sectionContent />

    <sectionIcon />

    <sectionJumbo />
  </main>
  <!-- /#site_main -->
  <footer id="site_footer"></footer>
  <!-- /#site_footer -->

</template>


<style lang="scss">

</style>