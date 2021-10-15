<template>
  <section class="container mx-auto pb-20 xl:p-10">
    <div class="lg:relative hero contact-hero">
      <contact-form class="mx-auto lg:absolute lg:bottom-10 lg:left-10 p-10 lg:p-5 bg-white max-w-md space-y-7 rounded z-10" />
      <iframe
        class="map grey-filter"
        src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d11972.750851358536!2d2.1863953218131864!3d41.39172964540061!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x12a4a2fd439609e1%3A0x42386118e65a3d70!2sCiutadella%20Park!5e0!3m2!1sen!2ses!4v1628602537402!5m2!1sen!2ses"
        allowfullscreen="true"
        width="100%"
        height="100%"
        loading="lazy"
      ></iframe>
    </div>
  </section>
</template>

<script>
export default {
  name: 'ContactUs'
}
</script>

<style>
</style>