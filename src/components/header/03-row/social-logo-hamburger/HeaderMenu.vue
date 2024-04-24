<script lang="ts" setup>
import './header-menu.scss'
import { setDarkMode } from '@/utils/utils'

import { ref } from 'vue'
import RightNav from '@/components/sliders/right-nav/RightNav.vue'
import HamburgerHorizontal from '@/components/icons/header/HamburgerHorizontal.vue'
import SunSvg from '@/components/icons/header/SunSvg.vue'
import MoonSvg from '@/components/icons/header/MoonSvg.vue'
import FacebookCircle from '@/components/icons/header/FacebookCircle.vue'
import TwitterCircle from '@/components/icons/header/TwitterCircle.vue'
import InstagramCircle from '@/components/icons/header/InstagramCircle.vue'

const isDarkMode = ref(localStorage.getItem('isDarkMode') === 'true')

const isRightNavOpen = ref<boolean | undefined>(undefined)

setDarkMode(isDarkMode.value)

const handleTheme = () => {
  isDarkMode.value = !isDarkMode.value
  setDarkMode(isDarkMode.value)
}

const toggleRightNav = () => {
  isRightNavOpen.value = !isRightNavOpen.value
}

</script>

<template>
  <nav class="header-menu-container">

    <div class="social">
      <FacebookCircle class="icon" />
      <TwitterCircle class="icon" />
      <InstagramCircle class="icon" />
    </div>

    <img src="/images/header/logos/logo-mps2.png" class="logo" alt="logo mps" />

    <div class="menu">

      <MoonSvg v-if="!isDarkMode" @click="handleTheme" class="icon sun" />
      <SunSvg v-else @click="handleTheme" class="icon moon" />

      <HamburgerHorizontal @click="toggleRightNav" class="icon desktop-only" />
      <RightNav :toggleRightNav="toggleRightNav" :isRightNavOpen="isRightNavOpen" />
    </div>

  </nav>
</template>
