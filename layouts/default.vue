<template>
  <div
    id="refineria-web"
  >
    <header-web />
    <nuxt />
    <footer-web />
  </div>
</template>

<script>
import HeaderWeb from '@/components/layout/HeaderWeb.vue'
import FooterWeb from '@/components/layout/FooterWeb.vue'

export default {
  components: { HeaderWeb, FooterWeb },
  name: 'default'
}
</script>

<style>
</style>