<template>
  <footer class="bg-gray-900 p-5 py-20 lg:py-40">
    <div class="container mx-auto flex justify-center border-gray-600 border-b pb-20">
      <div class="max-w-5xl space-y-4 text-center text-white">
        <h2 class="text-3xl sm:text-5xl font-bold"> Comencemos</h2>
        <p class="font-serif text-lg sm:text-2xl">Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
        <div class="flex justify-center">
          <button class="flex items-center py-4 px-24 sm:px-36 rounded font-bold text-xl transition duration-500 ease-in-out bg-indigo-600 hover:bg-indigo-500 transform hover:-translate-y-1 hover:scale-110">
            <img
              class="w-8 mr-2"
              src="../../static/svg-icons/whatsapp.svg"
              alt="&#128222;"
            >
            Contactar
          </button>
        </div>
      </div>
    </div>
    <div class="max-w-lg mx-auto flex justify-between text-gray-500 text-lg pt-20 font-serif">
      <nuxt-link to="#"> Proyectos </nuxt-link>
      <nuxt-link to="#"> Promociones </nuxt-link>
      <nuxt-link to="#"> Quiénes Somos </nuxt-link>
    </div>
    <social-networks />
    <p class="text-gray-500 text-center text-lg mt-12"> 15 Tips to Increase Your Adwords Profits </p>
    <div class="flex justify-center mt-12">
      <img
        src="../../static/footer-logo.png"
        alt="Refineria Web"
      >
    </div>
  </footer>
</template>

<script>
import SocialNetworks from '../SocialNetworks.vue'
export default {
  name: 'FooterWeb',
  components: {
    SocialNetworks
  }
}
</script>

<style>
</style>