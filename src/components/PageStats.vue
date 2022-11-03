<template>
  <div class="stats flex flex-col justify-center items-center">
    <h2 class="title mb-7">The leading customers agent in Europe and UK</h2>
    <hr class="w-14 h-[3px] bg-white lg:bg-[#059CB6] border-none mb-9" />
    <div
      class="stats-inner flex justify-between flex-col lg:flex-row w-full lg:w-3/4"
    >
      <div class="flex flex-col items-center justify-center">
        <h3 class="amount">20 +</h3>
        <h6 class="description">years of experience</h6>
      </div>
      <span class="vertical-divider item h-24 bg-green-50 ml-9"></span>
      <div class="flex flex-col items-center justify-center">
        <h3 class="amount">400</h3>
        <h6 class="description">qualified customs specialists</h6>
      </div>
      <span class="vertical-divider item h-24 bg-green-50 ml-9"></span>
      <div class="flex flex-col items-center justify-center">
        <h3 class="amount">20</h3>
        <h6 class="description">strategic locations</h6>
      </div>
      <span class="vertical-divider item h-24 bg-green-50 ml-9"></span>
      <div class="flex flex-col items-center justify-center">
        <h3 class="amount">5</h3>
        <h6 class="description">countries</h6>
      </div>
    </div>
    <BaseButton class="mt-10 w-5/6 sm:w-3/4 lg:w-auto">
      <template> Get in touch </template></BaseButton
    >
  </div>
</template>

<script>
import BaseButton from "./Base/BaseButton.vue";
export default {
  name: "PageStats",
  components: {
    BaseButton,
  },
};
</script>

<style lang="css" scoped>
.stats {
  background-color: #006b6e;
  padding: 75px;
  color: white;
}
.stats .title {
  font-size: 30px;
  font-weight: 700;
}
.stats .stats-inner .amount {
  font-size: 50px;
  font-weight: 700;
}
.stats .stats-inner .description {
  font-size: 20px;
  font-weight: 700;
}
.stats .vertical-divider {
  width: 1px;
  opacity: 0.4;
}
@media only screen and (max-width: 1022px) {
  .stats {
    padding: 75px 32px;
  }
  .stats .vertical-divider {
    height: 1px;
    width: 100%;
    margin: 40px 0px;
  }
}
</style>
