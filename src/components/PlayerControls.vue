<template>
  <div class="player-controls__buttons">
    <button
      class="control-button"
      @click="shuffleAction()"
      :class="{ 'control-button--active': shuffle, 'control-button--active-dot': shuffle }"
    >
      <ShuffleIcon />
    </button>
    <button class="control-button">
      <PreviousIcon />
    </button>
    <play-pause-button />
    <button class="control-button">
      <NextIcon />
    </button>
    <button
      class="control-button"
      @click="repeatAction()"
      :class="{ 'control-button--active': repeat, 'control-button--active-dot': repeat }"
    >
      <RepeatIcon />
    </button>
  </div>
</template>

<script>
import PlayPauseButton from './PlayPauseButton.vue'

import ShuffleIcon from '../assets/icons/shuffle.svg'
import PreviousIcon from '../assets/icons/previous.svg'
import NextIcon from '../assets/icons/next.svg'
import RepeatIcon from '../assets/icons/repeat.svg'

export default {
  name: 'PlayerControls',
  components: {
    PlayPauseButton,
    ShuffleIcon,
    PreviousIcon,
    NextIcon,
    RepeatIcon
  },
  data () {
    return {
      shuffle: false,
      repeat: false
    }
  },
  methods: {
    shuffleAction () {
      this.shuffle = !this.shuffle
      return this.shuffle
    },
    repeatAction () {
      this.repeat = !this.repeat
      return this.repeat
    }
  }
}
</script>
