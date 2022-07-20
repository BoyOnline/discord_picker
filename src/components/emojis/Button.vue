<template>
    <div :style="`background-image: url(${sources.emoji})`" style="backgroundPosition: -132px -44px"
        class="vue3-discord-emojipicker__emojibutton cursor-pointer grayscale hover:filter-none hover:scale-110 transition-transform duration-150 ease-in-out"
        @mouseleave="newEmoji">
    </div>
</template>

<script setup>
defineProps({
    sources: {
        type: Object,
        required: true
    }
})

const newEmoji = ({ target }) => {
    const column = (Math.floor(Math.random() * 11)) * -22
    const row = (Math.floor(Math.random() * 4)) * -22

    target.style.backgroundPosition = `${column}px ${row}px`
}
</script>

<style lang="scss">
</style>