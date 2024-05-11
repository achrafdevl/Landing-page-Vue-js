<script setup>
  const links = [
    { name: 'Home', url: "#", active: true },
    { name: 'App', url: "#"},
    { name: 'Feautures', url: "#"},
    { name: 'Testimonials', url: "#"},

  ]
</script>

<template>
  
  <header class="">
    <nav class=" =container flex justify-between items-center">
      <div class="flex justify-between gap-20">
        <!-- logo -->

        <a href="#">VueDesing</a>

        <!-- navBar -->
        <div  class=" flex items-center text-xl gap-2">

          <a
            :href="link.url"
            class="px-4 py-3 bg-pink-50"
            v-for="(link, index) in links"
            :key="index"
            :class="{'text-indigo-900 font-bold': link.active}"
          >
            {{ link.name }}
          </a>

          <a href="#">
            About
          </a>

          <a href="#">
            Contact
          </a>

        </div>

      </div>
      
      <!--  -->
      <a href="#">
        Get Started
      </a>
      
    </nav>
  </header>

</template>

<style scoped>

</style>