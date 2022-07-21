<template>
 <div>

  <ProductHeader />


    <div class="w-full py-28 " id="Our_menu">

        <div class="pb-10 text-center">
          <h1 class="text-black font-bold text-5xl">Our menu</h1>
          <p class="text-xl">What would u like to eat?</p>
        </div>
        
        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 xl:grid-cols-4 px-10">

          <FoodPreview v-for="item in preview" :key="item.id"
              :desc="item.desc"
              :pic="item.pic"
              :btn="'Order'"
           

          />

        </div>
      
    
    </div>

    <div class="w-full  bg-no-repeat bg-cover bg-center" :style="{backgroundRepeat: 'no-repeat' + ';' , backgroundImage: 'url(' + require('@/assets/images/productbackground2.jpg') +')'}">
      <div class="bg-black bg-opacity-80">

        <div class="pt-10 pb-72">

           <div class="text-white py-4">
              <h1 class=" text-center font-bold text-5xl">Subscribe to Our Newsletter </h1>  
           </div>

          <div class="text-white flex">

              <div class=" border rounded-full bg-white mt-28 ml-2 flex justify-between md:mx-auto md:pl-4 items-center">
                  
                  <input type="text"  class="outline-none text-black text-xl md:text-2xl font-semibold text-center" placeholder="Enter your Email">
                                   
                  <div class="">
                      <button class="bg-gray-500 p-4 border rounded-full text-white text-2xl font-bold hover:border-2 hover:bg-black">Subscribe</button>
                  </div>
              </div>

          </div>

        </div>
       
      </div>
    </div>
            
 </div>
 
</template>

<script>

 export default{
   
   data(){
     return{
       preview: [

          {
            id:1,
            pic: require('@/assets/food/food1.jpg'),
            desc:`Lorem ipsum`
          },

          {
            id:2,
            pic: require('@/assets/food/Food3.jpg'),
            desc:`Lorem ipsum`
          
          },

          {
            id:3,
            pic: require('@/assets/food/food8.jpg'),
            desc:`Lorem ipsum`
          },

          {
            id:4,
            pic: require('@/assets/food/food9.jpg'),
            desc:`Lorem ipsum`
          },
          
          {
            id:5,
            pic: require('@/assets/food/food7.jpg'),
            desc:`Lorem ipsum`
          },

          {
            id:6,
            pic: require('@/assets/food/food10.jpg'),
            desc:`Lorem ipsum`
          },

          {
            id:7,
            pic: require('@/assets/food/Food5.jpg'),
            desc:`Lorem ipsum`
          },

          {
            id:8,
            pic: require('@/assets/food/Food4.jpg'),
            desc:`Lorem ipsum`
          },

       ] 

     };
   }

 }

</script>

<style>
  
</style>