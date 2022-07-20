<template>
  <div class="flex w-screen h-screen justify-center" style="
      background-color: #f4d03f;
      background-image: linear-gradient(132deg, #f4d03f 0%, #16a085 100%);
    ">
    <DiscordPicker class="absolute bottom-1/4" />
  </div>
</template>

<script setup>
import DiscordPicker from './components/DiscordPicker.vue';
</script>

<style scoped>
</style>
