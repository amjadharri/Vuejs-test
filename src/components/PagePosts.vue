<template>
  <div class="posts">
    <div class="grid grid-cols-1 lg:grid-cols-2">
      <img
        src="../assets/Bildschirmfoto 2021-01-08 um 16.31.19@2x.png"
        alt=""
      />
      <div class="post flex flex-col justify-center px-8 py-8 xl:pl-28">
        <h2 class="post-title text-[#3D4D62] font-bold">
          Lorem ipsum dolor sit amet
        </h2>
        <hr class="w-14 h-[3px] bg-[#059CB6] border-none my-7" />
        <p class="post-description text-base text-[#3D4D62] w-11/12 xl:w-2/3">
          Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam
          nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat,
          sed diam voluptua. At vero eos et accusam et justo duo dolores et ea
          rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem
          ipsum dolor sit amet. Lorem ipsum dolor sit amet, consetetur
          sadipscing elitr.
        </p>
      </div>
    </div>
    <div class="grid grid-cols-1 lg:grid-cols-2">
      <img
        class="block lg:hidden"
        src="../assets/Bildschirmfoto 2021-01-08 um 16.31.19@2x.png"
        alt=""
      />
      <div class="post flex flex-col justify-center px-8 py-8 xl:pl-60">
        <h2 class="post-title text-[#3D4D62] font-bold">
          Lorem ipsum dolor sit amet
        </h2>
        <hr class="w-14 h-[3px] bg-[#059CB6] border-none my-7" />
        <p class="post-description text-base text-[#3D4D62] w-11/12 xl:w-2/3">
          Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam
          nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat,
          sed diam voluptua. At vero eos et accusam et justo duo dolores et ea
          rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem
          ipsum dolor sit amet. Lorem ipsum dolor sit amet, consetetur
          sadipscing elitr.
        </p>
        <BaseButton class="w-full lg:w-max mt-6">
          <template> More information </template>
        </BaseButton>
      </div>
      <img
        class="hidden lg:block"
        src="../assets/Bildschirmfoto 2021-01-08 um 16.31.19@2x.png"
        alt=""
      />
    </div>
  </div>
</template>

<script>
import BaseButton from "./Base/BaseButton.vue";

export default {
  name: "PagePosts",
  components: { BaseButton },
};
</script>

<style lang="css" scoped>
.posts .post .post-title {
  font-size: 30px;
}
</style>
