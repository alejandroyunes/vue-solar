<script lang="ts" setup>
import './footer-contact.scss'
const year = new Date().getFullYear()

</script>


<template>
  <section>
    <div class="footer-container">
      <router-link class="link" to="/">
        <img src="/images/header/logos/solar-logo.png" alt="alt" width="200px" height="54px" />
      </router-link>

      <div class="address">
        <p class="title">Office</p>
        <p class="info">Grützenstrasse 18807 FreienbachSchweiz</p>
        <a class="tel" href="tel:+41787746337">+41 78 774 63 37</a>
        <a class="tel" href="mailto:matthias.schulz@estrella-immobilien.ch">matthias.schulz@estrella-immobilien.ch</a>
      </div>

      <div class="links">
        <p class="title">Links</p>
        <ul class="list">
          <router-link class="link" to="/">
            <li class="item">
              <span class="span">Home</span>
            </li>
          </router-link>
          <router-link class="link" to="/about">
            <li class="item">
              <span class="span">About</span>
            </li>
          </router-link>
          <router-link class="link" to="/services">
            <li class="item">
              <span class="span">Services</span>
            </li>
          </router-link>
          <router-link class="link" to="/blog">
            <li class="item">
              <span class="span">Blog</span>
            </li>
          </router-link>
          <router-link class="link" to="/contact">
            <li class="item">
              <span class="span">Contact</span>
            </li>
          </router-link>
        </ul>
      </div>
    </div>
  </section>
</template>
