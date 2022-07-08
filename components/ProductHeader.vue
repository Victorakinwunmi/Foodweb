<template>

    <div class="w-full">
            <div class=" flex bg-black w-full justify-between opacity-80 fixed z-100">
                <div class="flex items-center">
                    <button :class="is_revealed ? 'hidden' : 'block lg:hidden' " class="pl-8 text-white" @click="showMenu">
                    <div>
                        <div class="bg-white h-1 w-5 px-5 my-2"></div>
                        <div class="bg-white h-1 w-5 px-5 my-2"></div>
                        <div class="bg-white h-1 w-5 px-5 my-2"></div>
                    </div>
                    </button>
        
                    <button :class="is_revealed ? 'block' :'hidden' " class="pl-8 text-white" @click="hideMenu">
                        <div>
                        <div class=" my-2 text-white">Back</div>
                        
                        </div>
                    </button>
                </div>

                <div class="">
                    <img :src="require('@/assets/images/logo.png')" class="w-full m-0 p-0">
                </div>

                <div :class="is_revealed ? 'block absolute top-14 bg-black text-center mt-10 h-screen' : 'hidden lg:flex' " class="text-white items-center justify-end px-28 w-full lg:flex lg:items-center">
                    
                    <nuxt-link to="/" class="p-6 block mx-auto lg:mx-0 lg:py-1  lg:flex lg:px-4 border-b-4 hover:border-white border-transparent  rounded-sm  duration-500 ease-in-out">Home</nuxt-link>
                    <nuxt-link to="product" class="p-6 block mx-auto lg:mx-0 lg:py-1  lg:flex lg:px-4 border-b-4 hover:border-white border-transparent  rounded-sm  duration-500 ease-in-out">Product</nuxt-link>
                    <nuxt-link to="/" class="p-6  px-0 block mx-auto lg:mx-0 lg:py-1  lg:flex lg:px-4 border-b-4 hover:border-white border-transparent  rounded-sm  duration-500 ease-in-out">About</nuxt-link>
                    <nuxt-link to="/" class="p-6 block mx-auto lg:mx-0 lg:py-1  lg:flex lg:px-4 border-b-4 hover:border-white border-transparent  rounded-sm  duration-500 ease-in-out">Contact</nuxt-link>
                    <nuxt-link to="/" class="p-2 block mx-auto lg:mx-0 lg:py-1  lg:flex lg:pl-8">Search icon</nuxt-link>
                    
                    
                </div>

            
    
            </div>

          
           <div class="w-full min-h-full bg-no-repeat bg-cover bg-center" :style="{backgroundRepeat: 'no-repeat' + ';' , backgroundImage: 'url(' + require('@/assets/images/productbackground.jpg') +')'}">
                <div class="bg-opacity-70 bg-black text-center">
                    <div class="py-48">
                        <div class="">
                            <h1 class=" text-white px-4 text-6xl lg:text-8xl font-black"> Welcome</h1>
                        </div>
                    
                        <div class="">
                            <h1 class="text-white px-4 text-2xl py-8">Eat good food and look fresh</h1>
                        </div>

                        <div class="px-8">
                          <a href="#Our_menu" class="border-2 bg-white text-black border-white p-4 px-8 rounded-full font-bold hover:border-black border-transparent  rounded-sm  duration-500 ease-in-out">Learn more</a>
                        </div>
                    
                    </div>
                    
                </div>
         
        </div>

     </div>

                    
        

</template>

<script>

export default {
    data() {
        return {
            is_revealed: false
        };
    },
    methods: {
        showMenu() {
            this.is_revealed = true;
        },
        hideMenu() {
            this.is_revealed = false;
        }
    },

    
}
</script>

<style>
 
</style>