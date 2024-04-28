<script lang="ts" setup>
import './billboard-fixed.scss'
import ArrowDoubleSvg from '@/components/icons/ArrowDoubleSvg.vue'
</script>

<template>
  <div class="billboard-fixed-container">

    <div class="billboard-info">

      <div class="title">
        <h1>SOLAR RENEWABLE ENERGY</h1>
      </div>

      <div class="slogan">

        <h2> Sun-powered
          <span class="light">solutions for a</span>
          <span class="span"> Sustainable world</span>
        </h2>

        <div class="arrow">
          <ArrowDoubleSvg class="icon" />
        </div>

      </div>
    </div>

  </div>
  <img class="image-billboard" src="/images/billboard/image.png" alt="alt" />
  <span class="overlay" />
</template>
