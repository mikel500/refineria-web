<template>
  <header class="text-white">
    <div class="bg-custom-back grid md:grid-cols-2 py-4">
      <div class="text-center md:pr-10 pb-2 sm:pb-0">
        <span class="text-xs">Lorem ipsum dolor sit amet</span>
      </div>
      <div class="md:pl-10 text-center text-xs md:text-base">
        <span class="md:mr-10"> +34 777 888 555 </span>
        <span class="md:hidden">/</span>
        <span class="md:ml-5"> +34 777 888 555 </span>
      </div>
    </div>
    <nav class="dark-blue-gradient">
      <div class="grid grid-cols-2">
        <div class="pl-5 md:pl-0">
          <!-- Website Logo -->
          <a
            href="#"
            class="flex items-center md:justify-center py-4 px-2"
          >
            <img
              src="logo.png"
              alt="Refineria Web"
            >
          </a>
        </div>
        <!-- Primary Navbar items -->
        <div class="hidden lg:flex items-center justify-center lg:space-x-5 xl:space-x-7 lg:pr-5 xl:pr-40 font-bold text-lg">
          <nuxt-link to="#">Quiénes Somos</nuxt-link>
          <nuxt-link to="#">Proyectos</nuxt-link>
          <nuxt-link to="#">Promociones</nuxt-link>
          <nuxt-link to="#">Contacto</nuxt-link>
        </div>
        <!-- Mobile menu button -->
        <div class="lg:hidden flex items-center justify-end pr-5 md:pr-20">
          <button @click="menuIsActive=!menuIsActive">
            <svg
              class="w-6 h-6 text-gray-50"
              fill="none"
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
              <path d="M4 6h16M4 12h16M4 18h16"></path>
            </svg>
          </button>
        </div>
      </div>
      <!-- mobile menu -->
      <transition name="fade">
        <div
          v-if="menuIsActive"
          class="relative"
        >
          <ul class="absolute bg-white text-blue-900 w-full space-y-5 p-5">
            <li>
              <nuxt-link to="#">Quiénes Somos</nuxt-link>
            </li>
            <li>
              <nuxt-link to="#">Proyectos</nuxt-link>
            </li>
            <li>
              <nuxt-link to="#">Promociones</nuxt-link>
            </li>
            <li>
              <nuxt-link to="#">Contacto</nuxt-link>
            </li>
          </ul>
        </div>
      </transition>
    </nav>
  </header>
</template>

<script>
export default {
  name: 'HeaderWeb',
  data () {
    return {
      menuIsActive: false
    }
  }

}
</script>

<style>
</style>