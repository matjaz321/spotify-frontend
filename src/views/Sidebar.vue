<template>
  <div class="sidebar">
    <div class="sidebar__container">
      <div class="sidebar-main">
        <div class="sidebar-main__header">
          <a
            class="sidebar-main__logo"
            href="/browse/featured"
          >
            <SpotifyLogo />
          </a>
        </div>
        <div class="sidebar-main__items">
          <ul>
            <li class="sidebar-group">
              <div class="sidebar-item">
                <a
                  href="/browse"
                  class="sidebar-link sidebar-link--active"
                >
                  <div class="sidebar-link-text-icon">
                    <!-- @todo toggle home icon hidden/shown class on link change -->
                    <div
                      class="icon sidebar-link-text-icon__icon"
                      style="display: none;"
                    >
                      <HomeInactive />
                    </div>
                    <div class="icon sidebar-link-text-icon__icon">
                      <HomeActive />
                    </div>
                    <span class="sidebar-link-text-icon__text">
                      Home
                    </span>
                  </div>
                </a>
              </div>
            </li>

            <li class="sidebar-group">
              <div class="sidebar-item">
                <a class="sidebar-link sidebar-link">
                  <div class="sidebar-link-text-icon">
                    <div class="icon sidebar-link-text-icon__icon">
                      <Search />
                    </div>
                    <span class="sidebar-link-text-icon__text">
                      Search
                    </span>
                  </div>
                </a>
              </div>
            </li>

            <li class="sidebar-group">
              <div class="sidebar-item">
                <a class="sidebar-link sidebar-link">
                  <div class="sidebar-link-text-icon">
                    <div class="icon sidebar-link-text-icon__icon">
                      <Library />
                    </div>
                    <span class="sidebar-link-text-icon__text">
                      Your library
                    </span>
                  </div>
                </a>
              </div>
            </li>
          </ul>
        </div>
      </div>
    </div>
    <div class="sidebar__signup signup-sidebar">
      <p>
        <button 
            class="btn btn--white btn--no-margin btn--full-width signup-sidebar--btn"
            @click="login"
        >
          Sign up
        </button>
      </p>
      <p>
        <button class="btn btn--black btn--no-margin btn--full-width signup-sidebar--btn">
          Log in
        </button>
      </p>
      <div class="signup-sidebar__text">
        <a
          href="https://www.spotify.com/legal/cookies-policy/"
          target="_blank"
          rel="noopener"
        >
          Cookies
        </a>
        <div class="signup-sidebar__split"></div>
        <a
          href="https://www.spotify.com/legal/cookies-policy/"
          target="_blank"
          rel="noopener"
        >
          Privacy
        </a>
      </div>
    </div>
  </div>
</template>

<script>
import SpotifyLogo from '../assets/icons/logo.svg'
import HomeInactive from '../assets/icons/HomeInactive.svg'
import HomeActive from '../assets/icons/HomeActive.svg'
import Search from '../assets/icons/Search.svg'
import Library from '../assets/icons/Library.svg'
import conifg from '../config'

export default {
  name: 'MainSidebar',
  components: {
    SpotifyLogo,
    HomeInactive,
    HomeActive,
    Search,
    Library
  },
  methods: {
    login() {
      window.location = config
    }
  }
}
</script>
