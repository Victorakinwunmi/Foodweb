<template>
 <div>

  <ProductHeader />


    <div class="w-full py-28 " id="Our_menu">

        <div class="pb-10 font-bold text-4xl text-center">
          <h1 class="text-black font-bold text-4xl">Our menu</h1>
        </div>
        
        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 px-10" id="grids">
          
                <div class="p-2 shadow-xl">
                  <img :src="require('@/assets/images/about1.jpeg')" class="m-0">
                </div>

                <div class="p-2 shadow-xl">
                  <img :src="require('@/assets/images/about1.jpeg')" class="m-0">
                </div>

                <div class="p-2 shadow-xl">
                  <img :src="require('@/assets/images/about1.jpeg')" class="m-0">
                </div>

                <div class="p-2 shadow-xl">
                  <img :src="require('@/assets/images/about1.jpeg')" class="m-0">
                </div>

                <div class="p-2 shadow-x lg:mt-6">
                  <img :src="require('@/assets/images/about1.jpeg')" class="m-0">
                </div>

                <div class="p-2 shadow-xl lg:mt-6">
                  <img :src="require('@/assets/images/about1.jpeg')" class="m-0">
                </div>

                <div class="p-2 shadow-xl lg:mt-6">
                  <img :src="require('@/assets/images/about1.jpeg')" class="m-0">
                </div>

                <div class="p-2 shadow-xl lg:mt-6">
                  <img :src="require('@/assets/images/about1.jpeg')" class="m-0">
                </div>

            

        </div>
    
    </div>

    <div class="w-full  bg-no-repeat bg-cover bg-center" :style="{backgroundRepeat: 'no-repeat' + ';' , backgroundImage: 'url(' + require('@/assets/images/send_in_orders.jpg') +')'}">
      <div class="bg-black bg-opacity-60">

        <div class="pt-10 pb-72">

           <div class="text-white py-4">
              <h1 class=" text-center font-bold text-5xl">Subscribe to Our Newsletter </h1>  
           </div>

          <div class="text-white flex w-full">

              <div class="mx-auto mt-28 block flex justify-between border px-auto md:pl-4 rounded-full bg-white items-center">
                  <input type="text"  class="outline-none text-black text-xl md:text-2xl font-semibold text-center" placeholder="Enter your Email">

                   <div class="">
                      <button class="border rounded-full py-4 px-10 bg-gray-500 text-white text-2xl font-bold">Subscribe</button>
                  </div>
              </div>

          </div>

        </div>
       
      </div>
    </div>
            
 </div>
 
</template>

<script>


</script>

<style>
  
</style>