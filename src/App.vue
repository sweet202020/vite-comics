<script>
import siteHeader from "./components/siteHeader.vue";
import comicList from "./components/comicList.vue";
import sectionContent from "./components/sectionContent.vue";
import sectionIcon from "./components/sectionIcon.vue";
import sectionJumbo from "./components/sectionJumbo.vue";
import FooterItem from "./components/FooterItem.vue";
export default {
  name: 'App',
  components: {
    siteHeader,
    sectionContent,
    comicList,
    sectionIcon,
    sectionJumbo,
    FooterItem,
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
  <FooterItem />
  <!-- /#site_footer -->

</template>


<style lang="scss">

</style>