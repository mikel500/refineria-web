<template>
  <div id="homepage">
    <div class="h-screen main-image md:h-full xl:h-screen flex justify-center">
      <div class="max-w-5xl pt-24 md:pt-56 md:pb-56 2xl:pt-80 text-center text-white px-6 md:py-0">
        <h1 class="text-4xl md:text-6xl font-bold"> Construimos tus sueños </h1>
        <p class="mt-12 text-lg md:text-2xl leading-loosen font-serif">Lorem ipsum dolor sit amet consectetur adipisicing elit. Saepe voluptatibus quod quo voluptatum blanditiis quia, animi consequuntur ullam modi fugiat exercitationem voluptate enim at!</p>
        <a class="w-full flex justify-center items-center mt-8 xl:mt-24 cursor-pointer">
          <img
            class="w-28"
            src="../static/svg-icons/chevron-down.svg"
            alt="&#8964;"
          >
        </a>
      </div>
    </div>
    <features />
    <CTAMeetDeadlines />
    <why-us-section />
    <CTAContactUs />
    <building-projects />
    <last-buildings />
    <contact-us />
  </div>
</template>

<script>

import ContactForm from '@/components/ContactForm'
import Features from '@/components/Features.vue'
import CTAMeetDeadlines from '@/components/CTAMeetDeadlines.vue'
import WhyUsSection from '@/components/WhyUsSection.vue'
import CTAContactUs from '@/components/CTAContactUs.vue'
import BuildingProjects from '@/components/BuildingProjects.vue'
import LastBuildings from '@/components/LastBuildings.vue'
import ContactUs from '@/components/ContactUs.vue'

export default {
  name: 'index',
  components: {
    ContactForm,
    Features,
    CTAMeetDeadlines,
    WhyUsSection,
    CTAContactUs,
    BuildingProjects,
    LastBuildings,
    ContactUs
  }
}
</script>

<style lang="scss">

.main-image {
  background: url("../static/building.webp"), linear-gradient(#182142, #193972);
  background-size: contain;
  background-repeat: no-repeat;
  background-position: right bottom;
  @media (max-width: 400px) {
    background-size: cover;
    background-position: center center;
  }
}

</style>