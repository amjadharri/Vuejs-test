<template>
  <div class="footer grid grid-cols-1 py-8 px-8 lg:px-0 w-full lg:w-3/4">
    <div
      class="flex flex-col w-full lg:max-w-none lg:flex-row items-start lg:items-center justify-between gap-0 lg:gap-11"
    >
      <a
        href=""
        class="footer-item relative text-base font-bold text-[#3D4D62] py-3"
      >
        Imprint</a
      >
      <a
        href=""
        class="footer-item relative text-base font-bold text-[#3D4D62] py-3"
      >
        Data security</a
      >
      <a
        href=""
        class="footer-item relative text-base font-bold text-[#3D4D62] py-3"
      >
        Conditions</a
      >
      <a
        href=""
        class="footer-item relative text-base font-bold text-[#3D4D62] py-3"
      >
        Cookies</a
      >
      <a href="" class="text-base font-bold text-[#3D4D62] py-3">
        Customs support</a
      >
    </div>
    <span
      class="text-xs text-start lg:text-end text-[#445667] w-full font-normal self-center mt-10 lg:mt-0"
      >© 2021 Customs Support Group. All rights reserved.</span
    >
  </div>
</template>

<script>
export default {
  name: "PageFooter",
};
</script>

<style lang="css" scoped>
.footer {
  margin: auto;
  grid-template-columns: 3fr 2fr;
}

@media only screen and (max-width: 1022px) {
  .footer {
    grid-template-columns: 1fr;
    place-items: center;
  }
  .footer .footer-item {
    width: 100%;
  }

  .footer .footer-item::after {
    content: "";
    width: 100%;
    height: 1px;
    background-color: #cccccc;
    position: absolute;
    bottom: 0;
    left: 0;
  }
}
</style>
