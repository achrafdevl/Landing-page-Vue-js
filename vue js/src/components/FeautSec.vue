<script setup>
    import AppStoreButton from './app-store-button.vue';
    import PlayStoreButton from './play-store-button.vue';
</script>

<template>
    <section class="py-20">
        <div class="container grid grid-cols-2 gap-40 mb-24">

            <!-- left img -->
            <div >
                <img src="https://images.unsplash.com/photo-1588693951525-7b0be0fc710f?q=80&w=1974&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt="Description of the image" class="h-[800px] bg-pink-50 rounded-3xl">
            </div>

            <!-- right sec -->
            <div class="space-y-7 mt-16">

                <div class="text-green-500 flex justify-start items-center gap-4">
                    <hr class="w-16 border-2 border-green-400"/>
                    <p class="text-xl">More than a streaming service</p>         
                </div>
                <h3 class="text-5xl">
                    You bring the passion. We bring the music.
                </h3>

                <p class="text-2xl opacity-70"> 
                    Check out original playlists hand-picked by our team of experts, or stream guest playlists curated by the
                    artists you Love.
                </p>

                <div class="opacity-70 space-y-10">

                    <div class="flex justify-start items-center gap-4">
                        <div class="w-14 h-14 bg-indigo-900/70 dark:bg-indigo-100/20 text-indigo-50  rounded-full flex justify-center items-center">
                            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" class="w-10 fill-current">
                                <path d="M12,1C7,1 3,5 3,10V17A3,3 0 0,0 6,20H9V12H5V10A7,7 0 0,1 12,3A7,7 0 0,1 19,10V12H15V20H18A3,3 0 0,0 21,17V10C21,5 16.97,1 12,1Z" />
                            </svg>
                        </div>
                        <p class="text-xl">High-fidelity sound quality</p>
                    </div>
                    <div class="flex justify-start items-center gap-4">
                        <div class="w-14 h-14 bg-indigo-900/70 dark:bg-indigo-100/20 text-indigo-50  rounded-full flex justify-center items-center">
                            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" class="w-10 fill-current">
                            <path d="M16.36,14C16.44,13.34 16.5,12.68 16.5,12C16.5,11.32 16.44,10.66 16.36,10H19.74C19.9,10.64 20,11.31 20,12C20,12.69 19.9,13.36 19.74,14M14.59,19.56C15.19,18.45 15.65,17.25 15.97,16H18.92C17.96,17.65 16.43,18.93 14.59,19.56M14.34,14H9.66C9.56,13.34 9.5,12.68 9.5,12C9.5,11.32 9.56,10.65 9.66,10H14.34C14.43,10.65 14.5,11.32 14.5,12C14.5,12.68 14.43,13.34 14.34,14M12,19.96C11.17,18.76 10.5,17.43 10.09,16H13.91C13.5,17.43 12.83,18.76 12,19.96M8,8H5.08C6.03,6.34 7.57,5.06 9.4,4.44C8.8,5.55 8.35,6.75 8,8M5.08,16H8C8.35,17.25 8.8,18.45 9.4,19.56C7.57,18.93 6.03,17.65 5.08,16M4.26,14C4.1,13.36 4,12.69 4,12C4,11.31 4.1,10.64 4.26,10H7.64C7.56,10.66 7.5,11.32 7.5,12C7.5,12.68 7.56,13.34 7.64,14M12,4.03C12.83,5.23 13.5,6.57 13.91,8H10.09C10.5,6.57 11.17,5.23 12,4.03M18.92,8H15.97C15.65,6.75 15.19,5.55 14.59,4.44C16.43,5.07 17.96,6.34 18.92,8M12,2C6.47,2 2,6.5 2,12A10,10 0 0,0 12,22A10,10 0 0,0 22,12A10,10 0 0,0 12,2Z" />
                            </svg>
                        </div>
                        <p class="text-xl">Anywhere, any moment</p>
                    </div>
                    <div class="flex justify-start items-center gap-4">
                        <div class="w-14 h-14 bg-indigo-900/70 dark:bg-indigo-100/20 text-indigo-50  rounded-full flex justify-center items-center">
                            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" class="w-10 fill-current">
                                <path d="M17,10.5V7A1,1 0 0,0 16,6H4A1,1 0 0,0 3,7V17A1,1 0 0,0 4,18H16A1,1 0 0,0 17,17V13.5L21,17.5V6.5L17,10.5Z" />
                            </svg>
                        </div>
                        <p class="text-xl">Videos and Livestreams</p>
                    </div>
                    

                </div>
                    
              
                <div class="flex items-center gap-4 text-white" >                            
                    <play-store-button />
                    <app-store-button />

                </div>

            </div>
        </div>
    </section>
</template>

  