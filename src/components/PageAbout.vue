<template>
  <div class="about relative">
    <div class="overlay z-0"></div>
    <div class="about-inner grid absolute h-full w-full lg:w-1/2 z-20">
      <div></div>
      <div
        class="flex flex-col items-start lg:justify-center justify-end px-8 lg:px-0 py-4"
      >
        <h2 class="title text-2xl lg:text-3xl text-[#FFFFFF] font-bold">
          Customs clearance after Brexit
        </h2>
        <hr class="w-14 h-[3px] bg-[#059CB6] border-none my-7" />
        <p class="text-[white] w-full text-sm md:text-base lg:w-3/4 mb-8">
          Since 4 years we are successfully helping our customers to prepare
          their business for Brexit. Our Bexit customs agents are always
          up-to-date with the latest customs regulations after Brexit and look
          forward to support you with Brexit customs procedures.
        </p>
        <BaseButton> Brexit and customs: get ready! </BaseButton>
      </div>
    </div>
    <div
      class="grid grid-cols-1 lg:grid-cols-2 absolute bottom-0 h-1/2 lg:h-full w-full z-10"
    >
      <div class="bg-[#006b6e] opacity-50"></div>
    </div>
  </div>
</template>

<script>
import BaseButton from "./Base/BaseButton.vue";

export default {
  name: "PageAbout",
  components: { BaseButton },
};
</script>

<style lang="css" scoped>
.about {
  background-image: url(../assets/Gruppe\ maskieren\ 6@2x.png);
  background-position: center;
  background-size: cover;
  width: 100%;
  min-height: 600px;
  height: 600px;
  margin-top: 100px;
}
.about .overlay {
  z-index: 0;
  position: absolute;
  top: 0;
  left: 0;
  height: 100%;
  width: 100%;
}
.about .about-inner {
  grid-template-columns: 2fr 5fr 1fr;
}
@media only screen and (max-width: 1022px) {
  .about {
    min-height: 800px;
  }
  .about .about-inner {
    grid-template-columns: 1fr;
  }
}
</style>
