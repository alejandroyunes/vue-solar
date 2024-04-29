<script lang="ts" setup>
import './right-nav.scss'
import ExitSvg from '@/components/icons/ExitSvg.vue'

import ArrowDownDropdownSvg from '@/components/icons/ArrowDownDropdownSvg.vue'
import router from '@/router'

interface Props {
  toggleRightNav: () => void
  isRightNavOpen: boolean | undefined
}

const { toggleRightNav, isRightNavOpen } = defineProps<Props>()

const handleClick = (url: string) => {
  toggleRightNav()
  router.push(url)
}

</script>

<template>
  <div
    :class="['right-nav-container', isRightNavOpen ? 'right-slide-in' : '', isRightNavOpen === false ? 'right-slide-out' : '']">
    <div class="right-nav-header">

      <img src="/images/header/logos/solar-logo.png" class="logo" alt="logo mps" />

      <div @click="toggleRightNav" class="animation-exit">
        <ExitSvg class="exit-icon" />
      </div>
    </div>

    <div class="right-nav-content">
      <ul class="list">
        <li class="item" @click="handleClick('/')">
          <span class="svg">
            <ArrowDownDropdownSvg class="icon" />
          </span>
          <p class="link">Home</p>
        </li>

        <li class="item" @click="handleClick('/about')">
          <span class="svg">
            <ArrowDownDropdownSvg class="icon" />
          </span>
          <p class="link">About</p>
        </li>

        <li class="item" @click="handleClick('/contact')">
          <span class="svg">
            <ArrowDownDropdownSvg class="icon" />
          </span>
          <p class="link">Contact</p>
        </li>

      </ul>

      <div class="contact">
        <p class="contact-tel"><a href="tel:+41787746337">+41 78 774 63 37</a></p>
        <p class="contact-email">
          <a href="mailto:matthias.schulz@estrella-immobilien.ch">matthias.schulz@estrella-immobilien.ch</a>
        </p>
      </div>
    </div>
  </div>

  <div v-if="isRightNavOpen" @click="toggleRightNav" class="right-nav-bg"></div>
</template>