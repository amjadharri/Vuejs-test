<template>
  <div id="app">
    <PageHeader></PageHeader>
    <PageHero></PageHero>
    <PageBrands></PageBrands>
    <PageStats></PageStats>
    <PagePosts></PagePosts>
    <PageServices></PageServices>
    <CustomerSupport></CustomerSupport>
    <PageAbout></PageAbout>
    <PageForm></PageForm>
    <PageFooter></PageFooter>
  </div>
</template>

<script>
import PageHeader from "./components/PageHeader.vue";
import PageHero from "./components/PageHero.vue";
import PageBrands from "./components/PageBrands.vue";
import PageStats from "./components/PageStats.vue";
import PagePosts from "./components/PagePosts.vue";
import PageServices from "./components/PageServices.vue";
import CustomerSupport from "./components/CustomerSupport.vue";
import PageAbout from "./components/PageAbout.vue";
import PageForm from "./components/PageForm.vue";
import PageFooter from "./components/PageFooter.vue";
export default {
  name: "App",
  components: {
    PageHeader,
    PageHero,
    PageBrands,
    PageStats,
    PagePosts,
    PageServices,
    CustomerSupport,
    PageAbout,
    PageForm,
    PageFooter,
  },
};
</script>

<style scoped>
#app {
  font-family: "IBM Plex Sans", sans-serif;
}
</style>
