<template>
  <div
    class="brands p-8 pb-12 lg:p-24 flex items-center justify-center gap-0 lg:gap-20 flex-wrap"
  >
    <div class="brands-img">
      <img src="../assets/Gruppe maskieren 10@2x.png" alt="" />
    </div>
    <div class="brands-description flex flex-col items-start">
      <h3 class="title text-[#3D4D62] mb-7 font-bold">Who we work with</h3>
      <hr class="w-14 h-[3px] bg-[#059CB6] border-none mb-9" />
      <p class="description text-[#3D4D62] text-base font-normal">
        We are the trusted partner for customs matters of <br />
        more than 7000 companies across Europe. Since 20 <br />
        years we successfully operate with customers from <br />
        small and large good owners to freight forwarders <br />
        and digital platforms across various industries.
      </p>
    </div>
  </div>
</template>

<script>
export default {
  name: "PageBrands",
};
</script>

<style scoped>
.brands .brands-img {
  width: 586px;
  height: 324px;
}
.brands .brands-description .title {
  color: #3d4d62;
  font-size: 30px;
  font-weight: 800px;
}
</style>
