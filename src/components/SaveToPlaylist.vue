<template>
    <button
        class="now-playing__ctrl-button control-button"
        :class="{'control-button--active': saved}"
        @click="chageStatus()"
    >
        <svg v-if="!saved" width="24" height="24" xmlns="http://www.w3.org/2000/svg" fill="currentColor"><path d="M11 11v-11h1v11h11v1h-11v11h-1v-11h-11v-1h11z"/></svg>
        <svg v-else width="24" height="24" xmlns="http://www.w3.org/2000/svg" fill="currentColor" fill-rule="evenodd" clip-rule="evenodd"><path d="M21 6.285l-11.16 12.733-6.84-6.018 1.319-1.49 5.341 4.686 9.865-11.196 1.475 1.285z"/></svg>
    </button>
</template>

<script>
export default {
    name: 'SaveToPlaylist',
    data() {
        return {
            saved: false,
        }
    },
    methods: {
        chageStatus() {
            return this.saved = !this.saved;
        },
    }
}
</script>
