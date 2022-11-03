<template>
  <button class="base-button text-base font-semibold rounded">
    <slot></slot>
  </button>
</template>

<script>
export default {
  name: "BaseButton",
};
</script>
<style>
.base-button {
  font-family: "IBM Plex Sans", sans-serif;
  background-color: #01a4b7;
  color: white;
  height: 50px;
  padding: 15px 30px;
}
.base-button:hover {
  background-color: #007e91;
}
</style>
