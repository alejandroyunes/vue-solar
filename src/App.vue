<script setup lang="ts">
import { ref } from 'vue'
import Header from '@/components/header/03-row/logo-menu-hamburger/HeaderComponent.vue'
import Footer from './components/footer/copyright-centered/FooterCopyright.vue'
import CookiesCompliance from './components/sections/01-row/cookies-compliance/CookiesCompliance.vue'

const cookiesAccepted = ref(localStorage.getItem('cookiesAccepted') === 'true' || false)


const handleCookies = () => {
  cookiesAccepted.value = true
  localStorage.setItem('cookiesAccepted', 'true')
}

</script>

<template>
  <Header />
  <RouterView />
  <Footer />
  <CookiesCompliance v-show="!cookiesAccepted" :handle-cookies="handleCookies" />
</template>
