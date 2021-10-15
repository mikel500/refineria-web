<template>
  <section class="bg-gray-100 px-5 py-20 xl:p-40">
    <div class="grid gap-10 lg:grid-cols-2 xl:grid-cols-4 justify-items-center container mx-auto">
      <article
        v-for="icon of icons"
        :key="icon"
        class="space-y-7 text-center"
      >
        <img
          class="w-12 h-12 mx-auto"
          :src="require(`../static/svg-icons/${icon}.svg`)"
          :alt="icon"
        >
        <h3 class="text-3xl md:text-4xl font-bold">Lorem ipsum</h3>
        <p class="font-serif text-gray-400">Lorem ipsum dolor sit amet consectetur adipisicing elit. Quod ullam, sit, quisquam sed rerum libero nesciunt ad nobis temporibus labore debitis esse. Facere, cum recusandae! Veritatis asperiores architecto nisi consectetur?</p>
      </article>
    </div>
  </section>
</template>

<script>
export default {
  name: 'WhyUsSection',
  data () {
    return {
      icons: ['lightning-bolt', 'badge-check', 'chat', 'home']
    }
  }
}
</script>

<style>
</style>