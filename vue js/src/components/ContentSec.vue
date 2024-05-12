<script setup>
 import { ref } from "vue";


    const content = ref( [
        {
            title: "Clearly hear the best sound offline.",
            description: "Malesuada nunc vel risus commodo viverra. Sed enim ut sem viverra. Nulla aliquet porttitor lacus luctus accumsan tortor compromises."

        },
        {
            title: "Elevate you sound.",
            description: "Malesuada nunc vel risus commodo viverra. Sed enim ut sem viverra. Nulla aliquet porttitor lacus luctus accumsan tortor compromises."

        },
        {
            title: "A world of music in your pocket.",
            description: "Malesuada nunc vel risus commodo viverra. Sed enim ut sem viverra. Nulla aliquet porttitor lacus luctus accumsan tortor compromises."

        },
    ])

</script>




<template>

     <!-- Second Section  -->

    <section class="py-20">

        <div class="container rounded-2xl bg-slate-50 dark:bg-indigo-800/20 py-10 space-y-7 px-10">
            <!-- Title -->

            <h2 class="text-5xl text-center">
                More than a streaming service
            </h2>

            <div class="flex justify-between items-start gap-10">
                <!-- left sec -->
                
                <div class="flex-1 gap-y-32 flex flex-col py-36 ">
                    
                    <div v-for="(item, index) in content" :key="index" class="space-y-7 max-w-sm">
                        
                        <p 
                        class="w-10 h-10  flex justify-center items-center rounded-full"
                        :class="index === 0 ? 'bg-blue-500 text-white' : 'bg-indigo-50 text-indigo-900'">
                            {{ index + 1 }}
                        </p>

                        <h3 class="text-3xl font-bold">
                            {{ item.title }}
                        </h3>
                        
                        <p class="">
                            {{ item.description }}
                        </p>
                    </div>
                </div>
                
                <!-- right sec -->
                
                <div class="flex-1 flex flex-col py-10">
                    <div class="h-96 max-w-sm bg-indigo-200 relative">
                        <div class="absolute top-10 -right-10 bg-white dark:bg-indigo-950 flex justify-between items-center rounded overflow-hidden">
                            <!-- <img src="/vue js/src/assets/" alt="phone"> -->
                            <div class="px-7 ">
                                <p class="font-bold text-1g">Morning Playlist</p>
                                <p class="font-thin">The best songs ever</p>
                            </div>
                            <img src="https://images.unsplash.com/photo-1505740420928-5e560c06d30e?q=80&w=100h=100&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt=""
                                class="w-28 h-20 bg-pink-50"

                            >
                            
                        </div>

                    </div>
                </div>
            </div>

        </div>


    </section>

</template>



    

             