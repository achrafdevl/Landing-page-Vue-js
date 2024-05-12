<script setup>
    import AppStoreButton from './app-store-button.vue';
    import PlayStoreButton from './play-store-button.vue';


  const links = [
    { name: 'Home', url: "#", active: true },
    { name: 'App', url: "#ContentSec", },
    { name: 'Feautures', url: "#FeautSec"},
    { name: 'Testimonials', url: "#TestiSec"},

  ]

</script>

<template>
  
  <!-- Header:> Logo navbar  -->

    <header class="sticky top-0 shadow shadow-indigo-50/20 z-10 bg-white dark:bg-indigo-900">
      <nav class="container flex justify-between items-center ">

        <div class="flex items-center gap-32">
          <!-- logo -->

          <a href="#" class="text-2xl font-bold" >VueWeb</a>

          <!-- navBar -->
          <div  class=" flex items-center text-xl gap-2">

            <a
              :href="link.url"
              class="px-4 py-4 hover:text-indigo-900 dark:hover:text-indigo-200"
              v-for="(link, index) in links"
              :key="index"
              :class="{'text-indigo-900 dark:text-indigo-50 font-bold': link.active}"
            >
              {{ link.name }}
            </a>

            

          </div>

        </div>
        
        <!--  -->
        <a href="#" class="flex items-center text-indigo-900 dark:text-indigo-50 font-bold px-7 py-4">
          <span>
            Get Started
          </span>
            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" class="w-10  fill-current">
              <path d="M14 16.94V12.94H5.08L5.05 10.93H14V6.94L19 11.94Z" />
            </svg>
        </a>
        
      </nav>
    </header>

  <!-- section 1 -->

    <section class="relative py-10">

      <div class="container grid grid-cols-2 gap-7 ">

          <!-- left sect -->
        <div class="py-8 space-y-10">

          <h1 class="text-7xl">
            You bring the passion. <br>  bring the music.
          </h1>
          <p class="text-2xl">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Quaerat suscipit voluptas, unde deserunt voluptatum incidunt ipsum explicabo eum omnis minus ducimus, accusantium iure? Numquam dolore iste tempora laboriosam nemo blanditiis.
          </p>
          
          <div class="flex items-center gap-4 text-white" >
            
            
            
            <play-store-button />
            <app-store-button />

          </div>
        
        </div> 

        <!-- right section -->
        <div class="absolute w-1/2  right-0 top-8 grid grid-cols-12 gap-2">

          <div class="h-40 bg-gray-400/20 col-start-1 col-end-3 "><img class="h-40 w-full" src="https://images.unsplash.com/photo-1534205643743-6737932c79ee?q=80&w=1974&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt=""></div>
          <div class="h-40 bg-gray-400/20 col-start-3 col-end-8 "><img class="h-40 w-full" src="https://images.unsplash.com/photo-1493225457124-a3eb161ffa5f?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt=""></div>
          <div class="h-40 bg-gray-400/20 col-start-8 col-end-12 "><img class="h-40 w-full" src="https://images.unsplash.com/photo-1470225620780-dba8ba36b745?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt=""></div>
          
          <div class="h-52 bg-gray-400/20 row-start-2 col-start-1 col-end-7 "><img class="h-52 w-full" src="https://images.unsplash.com/photo-1620704075906-27bfa0d54f3b?q=80&w=2071&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt=""></div>
          <div class="h-52 bg-gray-400/20 col-start-7 col-end-12 "><img class="h-52 w-full" src="https://images.unsplash.com/photo-1459749411175-04bf5292ceea?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt=""></div>

          <div class="h-48 bg-gray-400/20 row-start-3 col-start-1 col-end-3 "><img class="h-48 w-full" src="https://images.unsplash.com/photo-1620578077783-33e254311182?q=80&w=1935&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt=""></div>
          <div class="h-48 bg-gray-400/20 col-start-3 col-end-8 "><img class="h-48 w-full" src="https://images.unsplash.com/photo-1460723237483-7a6dc9d0b212?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt=""></div>
          <div class="h-48 bg-gray-400/20 col-start-8 col-end-12 "><img class="h-48 w-full" src="https://images.unsplash.com/photo-1525362081669-2b476bb628c3?q=80&w=1974&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt=""></div>

        </div>
        
      </div>
    </section>

</template>


<style scoped>

</style>