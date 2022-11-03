<template>
  <div class="page-hero md:px-10 h-screen">
    <div
      class="page-hero-inner pt-8 md:pt-20 flex max-h-max items-center justify-center flex-col gap-16 lg:gap-0 lg:flex-row"
    >
      <div class="intro text-red-200 lg:w-1/2 w-full px-8 md:px-20">
        <div class="flex flex-col lg:items-start items-center">
          <h1
            class="text-4xl lg:text-5xl text-white font-extrabold mb-8 text-left"
          >
            Headache on complex customs matters for your business?
          </h1>
          <hr class="w-14 h-[3px] bg-[#059CB6] border-none mb-9" />
          <p class="text-base text-[white] mb-8 text-left">
            Customs Support is your neutral full-service customs broker for
            complex customs matters with 20+ years of expertise in Europe and
            over 400 customs specialists who are happy to take the load off your
            mind!
          </p>
          <BaseButton class="hidden lg:block">
            <template> Get your quote now </template>
          </BaseButton>
        </div>
      </div>
      <div
        class="services text-[white] lg:w-1/2 w-full lg:pl-10 flex justify-center"
      >
        <div class="list-services px-8">
          <span class="flex items-center pb-8"
            ><i class="fa fa-check text-[#01a4b7]"></i>
            <p class="ml-3">
              Fast and accurate customs clearance delivery
            </p></span
          >
          <span class="flex items-center pb-8"
            ><i class="fa fa-check text-[#01a4b7]"></i>
            <p class="ml-3">IBM Plex Sans, Bold</p></span
          >
          <span class="flex items-center pb-8"
            ><i class="fa fa-check text-[#01a4b7]"></i>
            <p class="ml-3">
              Online and real-time control of customs processes
            </p></span
          >
        </div>
      </div>
      <BaseButton class="lg:hidden">
        <template> Get your quote now </template>
      </BaseButton>
    </div>
  </div>
</template>

<script>
import BaseButton from "../components/Base/BaseButton.vue";
export default {
  name: "PageHero",
  components: {
    BaseButton,
  },
};
</script>

<style lang="css" scoped>
.page-hero {
  background-image: url("../assets/Gruppe\ maskieren\ 1@2x.png");
  width: 100%;
  height: 690px;
  background-position: center;
}
@media only screen and (max-width: 1022px) {
  .page-hero {
    height: 100vh;
  }
}
</style>
