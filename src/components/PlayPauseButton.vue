<template>
  <button
    class="control-button control-button__pause-button"
    @click="togglePlayPause"
  >
    <template v-if="isPlaying">
      <PlayIcon/>
    </template>
    <template v-else>
      <PauseIcon />
    </template>
  </button>
</template>

<script>
import PlayIcon from '../assets/icons/play.svg'
import PauseIcon from '../assets/icons/pause.svg'
export default {
  name: 'PlayPauseButton',
  components: {
    PlayIcon,
    PauseIcon
  },
  data () {
    return {
      isPlaying: true
    }
  },
  methods: {
    togglePlayPause () {
      this.isPlaying = !this.isPlaying
      return this.isPlaying
    }
  }
}
</script>
