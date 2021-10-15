<template>
  <div>
    <h2 class="text-2xl lg:text-xl">Contacto </h2>
    <form class="grid grid-cols-1 gap-6">
      <label class="block">
        <span class="text-gray-700 font-bold">Nombre</span>
        <input
          type="text"
          placeholder="Mikel"
          class="p-2 mt-1 block w-full rounded-md bg-gray-100 border-transparent focus:border-gray-500 focus:bg-white focus:ring-0"
        >
      </label>
      <label class="block">
        <span class="text-gray-700 font-bold">Email</span>
        <input
          type="email"
          placeholder="lovecraft@gmail.com"
          class="p-2 mt-1 block w-full rounded-md bg-gray-100 border-transparent focus:border-gray-500 focus:bg-white focus:ring-0"
        >
      </label>
      <label class="block">
        <span class="text-gray-700 font-bold">Teléfono</span>
        <input
          type="text"
          placeholder="+34 636 636 636"
          class="p-2 mt-1 block w-full rounded-md bg-gray-100 border-transparent focus:border-gray-500 focus:bg-white focus:ring-0"
        >
      </label>
      <label class="block text-xs text-gray-400">
        <input type="checkbox">
        <span class="ml-1">He leído y acepto la clausula de protección de datos.</span>
      </label>
      <div class="text-center">
        <button
          type="button"
          class="py-3 w-36 bg-indigo-600 hover:bg-indigo-500 text-white"
          @click="submitForm"
        >
          Enviar
        </button>
      </div>
    </form>
  </div>
</template>

<script>
export default {
  name: 'ContactForm',
  methods: {
    async submitForm () {
      /*

       En resumidas cuentas en el método se enviaría la propiedad this.contactForm, en el caso de que las validaciones hayan ido correctamente.
       
       En Vue las validaciones se hacen con computadas. Ejemplo:
         errorName () {
          const name = this.form.name
          return name.length > 0 && name.length <= 100
         }

       Para hacer el post utilizaría axios: 
       const response = await this.$axios.$post('https://www.refineriaweb.com/contact-form', this.contactForm)

      Y puede que me espere algo así :) :
       
      $router->post('/contact-form', ['uses' => 'ContactController@store']);

      */
      console.log('Enviado')
    }
  }
}
</script>

<style>
</style>