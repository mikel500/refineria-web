<template>
  <section class="bg-gray-100 px-5 py-20 xl:p-40">
    <div class="grid gap-10 lg:grid-cols-3 justify-items-center container mx-auto">
      <article
        v-for="n in 3"
        :key="'feature_'+n"
        class="space-y-7"
      >
        <h3 class="text-3xl md:text-4xl font-bold">Lorem ipsum</h3>
        <hr class="w-48 bg-indigo-700 h-2">
        <p class="font-serif text-gray-400">Lorem ipsum dolor sit amet consectetur adipisicing elit. Quod ullam, sit, quisquam sed rerum libero nesciunt ad nobis temporibus labore debitis esse. Facere, cum recusandae! Veritatis asperiores architecto nisi consectetur?</p>
      </article>
    </div>
  </section>
</template>

<script>
export default {
  name: 'Features'
}
</script>

<style>
</style>