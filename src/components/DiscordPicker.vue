<template>
    <div id="discord-picker" class="w-9/12">
        <div></div>
        <div class="flex h-12 bg-[#2E3136] rounded-xl">
            <UploadButton />
            <input class="grow outline-none bg-transparent text-stone-200" placeholder="消息@Pico" />
            <div class="flex items-center mr-5">
                <gif-button class="mr-3" :sources="sources" />
                <emoji-button :sources="sources" />
            </div>
        </div>
    </div>
</template>

<script setup>
import { reactive } from "vue"
import UploadButton from "./upload/Button.vue"
import GifButton from "./gif/Button.vue"
import EmojiButton from "./emojis/Button.vue"

const sources = reactive({
    search: 'https://en-zo.dev/vue-discord-emojipicker/search.svg',
    gif: 'https://en-zo.dev/vue-discord-emojipicker/gif.svg',
    category: 'https://en-zo.dev/vue-discord-emojipicker/categories/%REPLACE%.svg',
    variation: 'https://en-zo.dev/vue-discord-emojipicker/variations/variation_%REPLACE%.svg',
    emoji: 'https://en-zo.dev/vue-discord-emojipicker/sprite_emojis.png'
})
</script>

<style lang="scss">
.vue3-discord-emojipicker__emojibutton {
    width: 23px;
    height: 22px;
    background-repeat: no-repeat;
    background-size: 243px 88px;
}
</style>