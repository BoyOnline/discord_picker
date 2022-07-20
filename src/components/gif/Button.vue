<template >
    <img :src="sources.gif" class="w-6 cursor-pointer hover:brightness-150 transition duration-150 ease-in-out"
        alt="Gif button" width="10" height="10">
</template>

<script setup>
defineProps({
    sources: {
        type: Object,
        required: true
    }
})
</script>

<style lang="scss">
</style>