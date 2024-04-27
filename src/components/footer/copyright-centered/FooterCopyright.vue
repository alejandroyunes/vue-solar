<script lang="ts" setup>
import './footer-copyright.scss'
const year = new Date().getFullYear()

</script>

<template>
  <section>
    <div class="footer-copyright">
      <p>&copy; {{ year }} All Rights Reserved.</p>
    </div>
  </section>
</template>
