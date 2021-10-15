<template>
  <section class="bg-gray-100 px-5 p-20 xl:p-40 flex justify-center">
    <div class="h-full container space-y-7">
      <h2 class="text-5xl font-bold text-center"> Proyectos</h2>
      <p class="text-gray-400 text-center">Lorem ipsum dolor sit amet consectetur adipisicing elit. Quod ullam, sit, quisquam sed rerum libero nesciunt ad nobis temporibus labore debitis esse.</p>
      <div class="grid justify-items-center gap-10 grid-cols-1 xl:grid-cols-3">
        <router-link
          v-for="(building,index) of buildings"
          :key="'building_'+index"
          class="h-96 w-full max-w-md flex flex-col justify-end building pl-7 pb-7"
          to="#"
        >
          <div :class="`background-${building.bg}`"></div>
          <h2 class="text-white text-lg font-bold"> {{building.title}}</h2>
          <p class="font-serif text-lg text-gray-700">{{building.location}}</p>
        </router-link>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'BuildingProjects',
  data () {
    return {
      buildings: [
        { title: 'Edificio número 4', location: 'Mallorca, España', bg: 'modern-building' },
        { title: 'Vista al Mar', location: 'Barcelona, España', bg: 'beach-building' },
        { title: 'Unifamiliares', location: 'Madrid, España', bg: 'house' }
      ]
    }
  }
}
</script>

<style lang="scss">

$buildings: ("modern-building", "beach-building", "house");

@each $building in $buildings {
  .building {
    position: relative;
    z-index: 1;
    background-color: rgba(132, 137, 147, 1);
    & .background-#{$building} {
      position: absolute;
      z-index: -1;
      top: 0;
      bottom: 0;
      left: 0;
      right: 0;
      background: url("../static/#{$building}.webp");
      background-size: cover;
      opacity: 0.3;
    }
  }
}
</style>