<template>
  <div
    class="customer-support flex flex-col relative px-8 w-full lg:w-3/4 mx-auto justify-center items-center text-center"
  >
    <h2 class="title text-[#3D4D62] font-bold">
      Customs Support is a full-service provider for customs services and is
      here to help
    </h2>
    <hr class="w-14 h-[3px] bg-[#059CB6] border-none my-7" />
    <div
      class="grid grid-cols-1 lg:grid-cols-3 gap-12 pb-12 mb-6 border-b border-gray-300"
    >
      <div class="flex flex-col items-start justify-center">
        <img src="../assets/Komponente 19 – 1@2x.png" alt="" />
        <h3 class="text-xl text-[#3D4D62] font-bold my-7">
          Import customs clearance
        </h3>
        <p class="text-base text-[#3D4D62] font-normal text-left mb-6">
          If you would like to import goods from a third country to within the
          European Union, Customs Support assists you in every step of the
          customs clearance process. Our customs experts take care of import
          documents, classification of import goods with the correct HS code,
          coordination of physical inspection and duty management.
        </p>
        <a href="" class="text-base font-bold text-[#01a4b7]"
          >Learn more <i class="fa fa-chevron-right ml-2 text-xs"></i
        ></a>
      </div>
      <div class="lg:flex hidden flex-col items-start justify-center">
        <img src="../assets/Komponente 19 – 1@2x.png" alt="" />
        <h3 class="text-xl text-[#3D4D62] font-bold my-7">
          Import customs clearance
        </h3>
        <p class="text-base text-[#3D4D62] font-normal text-left mb-6">
          If you would like to import goods from a third country to within the
          European Union, Customs Support assists you in every step of the
          customs clearance process. Our customs experts take care of import
          documents, classification of import goods with the correct HS code,
          coordination of physical inspection and duty management.
        </p>
        <a href="" class="text-base font-bold text-[#01a4b7]"
          >Learn more <i class="fa fa-chevron-right ml-2 text-xs"></i
        ></a>
      </div>
      <div class="lg:flex hidden flex-col items-start justify-center">
        <img src="../assets/Komponente 19 – 1@2x.png" alt="" />
        <h3 class="text-xl text-[#3D4D62] font-bold my-7">
          Import customs clearance
        </h3>
        <p class="text-base text-[#3D4D62] font-normal text-left mb-6">
          If you would like to import goods from a third country to within the
          European Union, Customs Support assists you in every step of the
          customs clearance process. Our customs experts take care of import
          documents, classification of import goods with the correct HS code,
          coordination of physical inspection and duty management.
        </p>
        <a href="" class="text-base font-bold text-[#01a4b7]"
          >Learn more <i class="fa fa-chevron-right ml-2 text-xs"></i
        ></a>
      </div>
    </div>
    <nav class="carousel flex gap-4 mt-4">
      <span
        class="carousel-item bg-[#01a4b7] rounded-full"
        type="radio"
        name="carousel-dots"
      ></span>

      <span
        class="carousel-item bg-slate-300 rounded-full"
        type="radio"
        name="carousel-dots"
      ></span>

      <span
        class="carousel-item bg-slate-300 rounded-full"
        type="radio"
        name="carousel-dots"
      ></span>
    </nav>
  </div>
</template>

<script>
export default {
  name: "CustomerSupport",
};
</script>

<style lang="css" scoped>
.customer-support {
  margin-top: 100px;
}
.customer-support::before {
  font-family: "Font Awesome 5 Free";
  font-weight: 900;
  font-size: 20px;
  content: "\f053";
  position: absolute;
  left: 0px;
  top: 370px;
  color: grey;
}
.customer-support::after {
  font-family: "Font Awesome 5 Free";
  font-weight: 900;
  font-size: 20px;
  content: "\f054";
  position: absolute;
  right: 0px;
  top: 370px;
  color: grey;
}
.customer-support .title {
  font-size: 30px;
}
.customer-support nav.carousel .carousel-item {
  width: 7px;
  height: 7px;
}
@media only screen and (max-width: px) {
}
</style>
