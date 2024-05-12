<script setup>

</script>


<template>
    <section class="py-20 bg-slate-200/20 dark:bg-indigo-800/10">
        <div class="container space-y-20">
            <div class="text-center space-y-3">
                <p>Join tens of thousands of music lovers</p>
                <h2 class="text-5xl">
                    What people say
                </h2>
            </div>

            
            <div class=" mx-auto container flex items-center gap-7">

                <div 
                    class=" flex flex-col items-center space-y-4 w-96 bg-white dark:bg-indigo-950 rounded-xl shadow  dark:shadow-indigo-800 p-8 "
                    v-for="i in 4"
                    :key="i"
                >
                
                    <img src="https://images.unsplash.com/photo-1552058544-f2b08422138a?q=80&w=100&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt="Testimonial 1" class="w-24 h-24 rounded-full"/>
                    <p class="text-xl font-semibold">John Doe</p>
                    <p class="text-sm text-gray-500">CEO at Company</p>
                    <p class="font-bold">Amazing sound !</p>
                    <p class="text-gray-600 text-center dark:text-indigo-200">
                        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed
                        viverra ipsum dolor, ultricies fermentum massa consequat eu.
                        Nullam nec elit eget dolor pretium semper vel vitae neque.
                    </p>
                    <div class="flex justify-center items-center gap-2">
                        <svg 
                            v-for="i in 5"
                            :key="i"
                            xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"
                            class="w-5 h-5 text-yellow-500 fill-current"
                        >
                            <path d="M12,17.27L18.18,21L16.54,13.97L22,9.24L14.81,8.62L12,2L9.19,8.62L2,9.24L7.45,13.97L5.82,21L12,17.27Z" />
                        </svg>
                    </div>

                </div>

            </div>
                    

        </div>
    </section>

</template>