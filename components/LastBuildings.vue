<template>
  <section class="px-5 py-20 xl:p-40 flex justify-center">
    <div class="h-full container space-y-7">
      <h2 class="text-5xl font-bold text-center"> Últimas promociones</h2>
      <p class="font-serif text-gray-500 text-center text-lg">Proyectos en marcha</p>
      <div class="grid justify-items-center gap-8 2xl:gap-0 grid-cols-1 xl:grid-cols-2">
        <router-link
          to="#"
          class="h-96 w-full max-w-xl flex flex-col justify-end building 2xl:ml-32 pl-7 pb-7"
        >
          <div class="background-house"></div>
          <h2 class="text-lg text-gray-600"> Septiembre 2020</h2>
          <p class="text-lg text-white font-bold">Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
        </router-link>
        <router-link
          to="#"
          class="h-96 w-full max-w-xl flex flex-col justify-end building 2xl:mr-32 pl-7 pb-7"
        >
          <div class="background-house"></div>
          <h2 class="text-lg text-gray-600"> Septiembre 2020</h2>
          <p class="text-lg text-white font-bold">Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
        </router-link>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'LastBuildings'
}
</script>

<style>
</style>