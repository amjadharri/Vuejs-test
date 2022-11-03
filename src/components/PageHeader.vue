<template>
  <nav class="bg-white mb-24">
    <div
      class="max-w-full sm:px-6 lg:px-0 fixed top-0 left-0 bg-white w-full z-50"
    >
      <div class="relative flex py-5 items-center justify-between px-6">
        <div
          class="flex items-center justify-center sm:items-center sm:justify-start"
        >
          <div class="flex flex-shrink-0 items-center">
            <img
              class="block h-10 w-auto lg:hidden"
              src="../assets/Logo@2x.png"
              alt="Your Company"
            />
            <img
              class="hidden h-12 w-auto lg:block"
              src="../assets/Logo@2x.png"
              alt="Your Company"
            />
            <span
              class="vertical-divider item h-10 sm:h-16 bg-slate-100 ml-6 sm:ml-8"
            ></span>
          </div>
          <div class="hidden sm:ml-6 sm:block">
            <div class="flex space-x-4 items-center">
              <a
                href="#"
                class="font-bold opacity-100 text-[#3d4d62] text-base px-3 py-2"
                aria-current="page"
                >Quick Facts
                <i
                  class="icon fa fa-chevron-down ml-2 text-[#01a4b7]"
                  aria-hidden="true"
                ></i>
              </a>

              <a
                href="#"
                class="font-bold opacity-100 text-[#3d4d62] text-base px-3 py-2"
                >Benefits
                <i
                  class="icon fa fa-chevron-down ml-2 text-[#01a4b7]"
                  aria-hidden="true"
                ></i
              ></a>

              <a
                href="#"
                class="font-bold opacity-100 text-[#3d4d62] text-base px-3 py-2"
                >Contact</a
              >
            </div>
          </div>
        </div>
        <div
          class="absolute inset-y-0 right-0 flex items-center pr-2 sm:static sm:inset-auto sm:ml-6 sm:pr-0"
        >
          <div class="absolute inset-y-0 right-6 flex items-center sm:hidden">
            <!-- Mobile menu button-->
            <button
              @click="menuOpen"
              type="button"
              :class="{ 'menu-open': menuOpen }"
              class="inline-flex items-center justify-center rounded-md p-2 text-gray-400 focus:outline-none focus:ring-2 focus:ring-inset focus:ring-white"
              aria-controls="mobile-menu"
              aria-expanded="false"
            >
              <span class="sr-only">Open main menu</span>
              <!--
          Icon when menu is closed.

          Heroicon name: outline/bars-3

          Menu open: "hidden", Menu closed: "block"
        -->
              <svg
                v-if="!menuOpen"
                @click="menuOpen = true"
                class="block h-6 w-6 text-[#01A4B7]"
                xmlns="http://www.w3.org/2000/svg"
                fill="none"
                viewBox="0 0 24 24"
                stroke-width="1.5"
                stroke="currentColor"
                aria-hidden="true"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  d="M3.75 6.75h16.5M3.75 12h16.5m-16.5 5.25h16.5"
                />
              </svg>
              <span v-if="menuOpen" @click="menuOpen = false">
                <i
                  class="fa fa-times font-light w-7 h-7 text-[#01A4B7]"
                  aria-hidden="true"
                ></i>
              </span>

              <!--
          Icon when menu is open.

          Heroicon name: outline/x-mark

          Menu open: "block", Menu closed: "hidden"
              -->
            </button>
          </div>
          <BaseButton class="hidden sm:block w-max">
            <template> Get in touch </template>
          </BaseButton>
          <!-- Profile dropdown -->
        </div>
      </div>
    </div>

    <div v-if="menuOpen == true" class="sm:hidden" id="mobile-menu">
      <div
        class="space-y-1 px-10 mt-20 pt-2 pb-6 flex flex-col items-center fixed inset-0 bg-white h-max"
      >
        <a
          href="#"
          class="text-[#3D4D62] w-full px-3 py-4 text-base font-bold border-b border-[#CCCCCC] text-center"
          aria-current="page"
          >Quick Facts
        </a>

        <a
          href="#"
          class="text-[#3D4D62] w-full px-3 py-4 text-base font-bold border-b border-[#CCCCCC] text-center"
          >Benefits</a
        >

        <a
          href="#"
          class="text-[#3D4D62] w-full px-3 py-4 text-base font-bold text-center"
          >Contact</a
        >
      </div>
    </div>
  </nav>
</template>

<script>
import BaseButton from "./Base/BaseButton.vue";
export default {
  name: "PageHeader",
  props: {
    msg: String,
  },
  components: {
    BaseButton,
  },
  data() {
    return {
      menuOpen: false,
    };
  },
};
</script>

<style scoped>
.page-header {
  padding: 20px 30px;
}
.page-header .left .item {
  margin-right: 49px;
}
.page-header .left .logo-img {
  width: 149px;
  height: 70px;
}
.vertical-divider {
  width: 2px;
}
</style>
