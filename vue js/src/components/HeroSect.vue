<script setup>
  const links = [
    { name: 'Home', url: "#", active: true },
    { name: 'App', url: "#"},
    { name: 'Feautures', url: "#"},
    { name: 'Testimonials', url: "#"},

  ]
</script>

<template>
  
  <!-- Header:> Logo navbar  -->

    <header class="sticky top-0 shadow shadow-indigo-50 ">
      <nav class="container flex justify-between items-center ">

        <div class="flex items-center gap-32">
          <!-- logo -->

          <a href="#" class="text-2xl font-bold" >VueWeb</a>

          <!-- navBar -->
          <div  class=" flex items-center text-xl gap-2">

            <a
              :href="link.url"
              class="px-4 py-4 hover:text-indigo-900"
              v-for="(link, index) in links"
              :key="index"
              :class="{'text-indigo-900 font-bold': link.active}"
            >
              {{ link.name }}
            </a>

            

          </div>

        </div>
        
        <!--  -->
        <a href="#" class="flex items-center text-indigo-900 font-bold px-7 py-4">
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

      <div class="container grid grid-cols-2 gap-7">

          <!-- left sect -->
        <div class="py-8 space-y-10">

          <h1 class="text-7xl">
            You bring the passion. <br>  bring the music.
          </h1>
          <p class="text-2xl">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Quaerat suscipit voluptas, unde deserunt voluptatum incidunt ipsum explicabo eum omnis minus ducimus, accusantium iure? Numquam dolore iste tempora laboriosam nemo blanditiis.
          </p>
          
          <div class="flex items-center gap-4 text-white" >
            
            <button class="flex justify-between items-center bg-blue-500 px-4 py-2 rounded-xl  gap-2"> 
              <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" class="w-14 fill-current">
                <path d="M3,20.5V3.5C3,2.91 3.34,2.39 3.84,2.15L13.69,12L3.84,21.85C3.34,21.6 3,21.09 3,20.5M16.81,15.12L6.05,21.34L14.54,12.85L16.81,15.12M20.16,10.81C20.5,11.08 20.75,11.5 20.75,12C20.75,12.5 20.53,12.9 20.18,13.18L17.89,14.5L15.39,12L17.89,9.5L20.16,10.81M6.05,2.66L16.81,8.88L14.54,11.15L6.05,2.66Z" />
              </svg>
  
  
              <span class="flex flex-col justify-start text-left">
                <span class="uppercase text-xs">Get it On</span>
                <span class="text-2xl">Google Play</span>
              </span>
            </button>
            
            <button class="flex justify-between items-center bg-gray-950 px-4 py-2 rounded-xl gap-2"> 
              <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" class="w-14 fill-current">
                <path d="M18.71,19.5C17.88,20.74 17,21.95 15.66,21.97C14.32,22 13.89,21.18 12.37,21.18C10.84,21.18 10.37,21.95 9.1,22C7.79,22.05 6.8,20.68 5.96,19.47C4.25,17 2.94,12.45 4.7,9.39C5.57,7.87 7.13,6.91 8.82,6.88C10.1,6.86 11.32,7.75 12.11,7.75C12.89,7.75 14.37,6.68 15.92,6.84C16.57,6.87 18.39,7.1 19.56,8.82C19.47,8.88 17.39,10.1 17.41,12.63C17.44,15.65 20.06,16.66 20.09,16.67C20.06,16.74 19.67,18.11 18.71,19.5M13,3.5C13.73,2.67 14.94,2.04 15.94,2C16.07,3.17 15.6,4.35 14.9,5.19C14.21,6.04 13.07,6.7 11.95,6.61C11.8,5.46 12.36,4.26 13,3.5Z" />            
              </svg>
  
              <span class="flex flex-col justify-start text-left">
                <span class="uppercase text-xs">Get it On</span>
                <span class="text-2xl">Apple Store</span>
              </span>
            </button>

          </div>
        
        </div> 

        <!-- right section -->
        <div class="absolute w-1/2  right-0 top-8 grid grid-cols-12 gap-2">

          <div class="h-40 bg-gray-400/20 col-start-1 col-end-3 "></div>
          <div class="h-40 bg-gray-400/20 col-start-3 col-end-8 "></div>
          <div class="h-40 bg-gray-400/20 col-start-8 col-end-12 "></div>
          
          <div class="h-52 bg-gray-400/20 row-start-2 col-start-1 col-end-7 "></div>
          <div class="h-52 bg-gray-400/20 col-start-7 col-end-12 "></div>

          <div class="h-48 bg-gray-400/20 row-start-3 col-start-1 col-end-3 "></div>
          <div class="h-48 bg-gray-400/20 col-start-3 col-end-8 "></div>
          <div class="h-48 bg-gray-400/20 col-start-8 col-end-12 "></div>

        </div>
        
      </div>
    </section>

</template>

<style scoped>

</style>