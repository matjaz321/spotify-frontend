<template>
  <div class="extra-controls">
    <div class="extra-controls--queue">
      <button class="control-button">
        <QueueIcon />
      </button>
    </div>
    <!-- @todo On slide volume control change icons -->
    <div class="extra-controls--volume">
      <div class="volume-bar">
        <button class="volume-bar--icon control-button">
          <SoundFull />
        </button>
        <div class="volume-bar__progress-bar progress-bar">
          <progress-bar />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import ProgressBar from './ProgressBar'

import QueueIcon from '../assets/icons/Queue.svg'
import SoundFull from '../assets/icons/SoundFull.svg'
export default {
  name: 'ExtraControls',
  components: {
    ProgressBar,
    QueueIcon,
    SoundFull
  },
  data () {
    return {

    }
  }
}

</script>
