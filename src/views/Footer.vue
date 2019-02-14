<template>
  <footer class="now-playing-bar" id="footer-playing-bar">
    <div class="now-playing-bar__container">
      <div class="now-playing-bar__inner-content">
        <div class="now-playing-bar__left">
          <now-playing/>
        </div>
        <div class="now-playing-bar__center">
          <div class="player-controls">
            <player-controls/>
            <div class="player-controls__playback playback-bar">
              <div class="playback-bar__progress-time">0:00</div>
              <progress-bar/>
              <div class="playback-bar__progress-time">3:22</div>
            </div>
          </div>
        </div>
        <div class="now-playing-bar__right">
          <div class="now-playing-right-inner">
            <extra-controls/>
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
  import NowPlaying from './../components/NowPlaying';
  import ProgressBar from './../components/ProgressBar';
  import ExtraControls from './../components/ExtraControls';
  import PlayerControls from './../components/PlayerControls';

  export default {
    name: 'Footer',
    components: {
      NowPlaying,
      ProgressBar,
      ExtraControls,
      PlayerControls,
    }
  }

</script>
