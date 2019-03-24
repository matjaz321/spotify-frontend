<template>
  <button
    class="now-playing__ctrl-button control-button"
    :class="{'control-button--active': saved}"
    @click="changeStatus"
  >
    <template v-if="!saved">
      <PlusIcon />
    </template>
    <template v-else>
      <CheckMarkIcon />
    </template>
  </button>
</template>

<script>
import PlusIcon from '../assets/icons/plus.svg'
import CheckMarkIcon from '../assets/icons/checkmark.svg'

export default {
  name: 'SaveToPlaylist',
  components: {
    PlusIcon,
    CheckMarkIcon
  },
  data () {
    return {
      saved: false
    }
  },
  methods: {
    changeStatus () {
      this.saved = !this.saved
      return this.saved
    }
  }
}
</script>
