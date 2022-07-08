<template>
  <div>
       <HomeHeader />

       
    
      <div class="w-full bg-gray-100">
      
        <div class="flex">
            <h1 class="font-bold text-2xl lg:text-4xl py-8 mx-auto text-black">Features Collections</h1>
        </div>

      </div>

      <div class="w-full grid grid-cols-1  xl:grid-cols-2 gap-6 mx-auto bg-gray-100">
       
        <div class="mx-auto">
          <img :src="require('@/assets/images/about2.jpg')" class="m-0 md:max-w-lg p-4">

          <div class="p-6 max-w-xl">
             diddhi Lorem ipsum dolor sit amet consectetur adipisicing elit. Sit possimus,
             necessitatibus dignissimos praesentium nesciunt nulla explicabo tenetur facilis adipisci
             diddhi Lorem ipsum dolor sit amet consectetur adipisicing elit. Sit possimus,
             necessitatibus dignissimos praesentium nesciunt nulla explicabo tenetur facilis adipisci  
           
          </div>
          
        </div>

        <div class="grid grid-cols-1 gap-6">
          <div class="items-center grid grid-cols-1 lg:grid-cols-2 ">
            <div class="max-w-md rounded-2xl mx-auto">
              <img :src="require('@/assets/images/about3.jpg')" class="w-full objec-fit m-0 p-4 rounded-2xl" />
            </div>
            <div class="p-10 lg:p-6">
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Velit deserunt, quam consequuntur veniam, 
                perferendis possimus earum, officiis magni autem deleniti beatae omnis iusto fugit reiciendis eveniet 
                veritatis suscipit assumenda laborum?
                iddhi Lorem ipsum dolor sit amet consectetur adipisicing elit. Sit possimus,
                necessitatibus dignissimos praesentium nesciunt nulla explicabo tenetur facilis adipisci 
            </div>
            
          </div>

          <div class="items-center grid grid-cols-1 lg:grid-cols-2 ">
            
            <div class="p-10 lg:p-6">
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Velit deserunt, quam consequuntur veniam, 
                perferendis possimus earum, officiis magni autem deleniti beatae omnis iusto fugit reiciendis eveniet 
                veritatis suscipit assumenda laborum?
                iddhi Lorem ipsum dolor sit amet consectetur adipisicing elit. Sit possimus,
                necessitatibus dignissimos praesentium nesciunt nulla explicabo tenetur facilis adipisci 
            </div>

            <div class="max-w-md rounded-2xl mx-auto">
              <img :src="require('@/assets/images/about1.jpeg')" class="w-full objec-fit m-0 p-4 rounded-2xl" />
            </div>
            
          </div>


        
        </div>


      </div>
      
      <div class="w-full" id="about">

          <div class="text-black text-4xl font-bold px-10 pt-10">

            <h1 class="">About Us</h1>

          </div>

      
       
        <div class="w-full grid grid-1 xl:grid-cols-3 gap-6 p-10"> 


          <Newsletter v-for="item in news" :key="item.id"
            :title="item.title"
            :paragraph="item.desc"
            :btn="'Read more'"
            :pic="item.pic"
          />

        </div>
             
        
      </div>
         
        
      <div class="w-full grid grid-1 xl:grid-cols-2 gap-6 p-10 pt-10">
        
      
          <div class="border border-white border-2 p-4 md:p-16 shadow-2xl">

            <div class="py-4 font-bold">
                Lorem ipsum dolor sit, amet consectetur adipisicing elit. Dignissimos iste incidunt et voluptatem 
                ipsa? Alias inventore, quisquam dolores provident

            </div>
            <div class="pt-2">
              Lorem ipsum dolor sit, amet consectetur adipisicing elit. Sit minima non odio, eveniet, omnis minus  
              illum nostrum ullam magni sunt asperiores assumenda perferendis corporis adipisci 
              laudantium porro similique placeat alias?
              Lorem ipsum dolor sit, amet consectetur adipisicing elit. Sit minima non odio, eveniet, omnis minus  
              illum nostrum ullam magni sunt asperiores assumenda perferendis corporis adipisci 
              laudantium porro similique placeat alias?
              Lorem ipsum dolor sit, amet consectetur adipisicing elit. Sit minima non odio, eveniet, omnis minus  
              illum nostrum ullam magni sunt asperiores assumenda perferendis corporis adipisci 
              laudantium porro similique placeat alias?
               Lorem ipsum dolor sit, amet consectetur adipisicing elit. Sit minima non odio, eveniet, omnis minus  
              illum nostrum ullam magni sunt asperiores assumenda perferendis corporis adipisci 
              laudantium porro similique placeat alias?
             dantium porro similique placeat alias?
              
            </div>
              
              <div class="pt-6 md:text-center sm:text-left lg:text-text-center xl:text-left">
                <button class="border-2 border-black text-black font-bold p-2 rounded-md hover:text-red-500">Read more</button>
              </div>
          </div>

          <div class="border border-white border-2 p-6 bg-gray-100">

            <div>
              <input type="text" placeholder="Full name" class="border-2 border-white p-2 w-full py-4 outline-none">
              <input type="number" placeholder="Mobile number" class="border-2 border-white mt-6 mr-4  w-full lg:w-5/12 p-2 py-4 outline-none ">
              <input type="email" placeholder="Email address"  class="border-2 border-white mt-6  w-full lg:w-5/12 p-2 py-4 outline-none ">
              <input type="text" placeholder="Gender" class="border-2 border-white mt-6 mr-4 w-full lg:w-5/12 p-2 py-4 outline-none ">
              <input type="number" placeholder="Age" class="border-2 border-white mt-6 w-full lg:w-5/12 p-2 py-4 outline-none ">
            </div>
           
            <div class="">
                <h1 class="font-bold text-2xl md:text-3xl text-gray-500 mt-10 mb-10">How can we help you?</h1>
            </div>      

            <div class="">
              <textarea class="w-full outline-none p-2 text-md" rows="5"></textarea>
            </div>

            <div class="text-center mt-10">
               <button class="border-2 bg-green-500 p-4 px-10 text-white font-bold hover:text-gray-500">Send us message</button>

            </div>
           

          </div>

      </div>

      <div class=" img" id="contacts">
        <div class="w-full bg-black opacity-80">

          <div class="p-16 text-center">
            <h1 class="font-bold text-4xl mb-10 text-white">Contact us on :</h1>

            <div class="w-full ">

              <div class="text-white font-bold mb-6 text-xl">
                 <div>
                   <h1></h1>
                 </div>

                 <div>
                  08104782750
                 </div>
              </div>
              
              <div class="text-white font-bold mb-6 text-xl">
                 <div>
                   <h1></h1>
                 </div>

                 <div>
                  @victoradedapo
                 </div>
              </div>

              <div class="text-white font-bold text-xl">
                 <div>
                   <h1></h1>
                 </div>

                 <div>
                  @Adex_victor12
                 </div>
              </div>

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
            is_revealed: false,
          
            news: [
              {
                id: 1,
                title: "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Dignissimos iste incidunt et volupt ipsa? Alias inventore",
                desc: `
                Lorem ipsum dolor sit, amet consectetur adipisicing elit. Sit minima non odio, eveniet, omnis m illum 
                nostrum ullam magni sunt asperiores assumenda perferendis corporis adipiscilaudantium porro similique placeat
                 alias?Lorem ipsum dolor sit, amet consectetur adipisicing elit. Sit minima non odio, eveniet, 
                omnis minus  illum nostrum ullam magni sunt asperiores assumenda perferendis corporis adipisci  laudantium porro similique placeat alias`,
                pic: require('@/assets/images/about1.jpeg')
              },

              {
                id: 2,
                title: "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Dignissimos iste incidunt et volupt ipsa? Alias inventore",
                desc: `
                Lorem ipsum dolor sit, amet consectetur adipisicing elit. Sit minima non odio, eveniet, omnis m illum 
                nostrum ullam magni sunt asperiores assumenda perferendis corporis adipiscilaudantium porro similique placeat
                 alias?Lorem ipsum dolor sit, amet consectetur adipisicing elit. Sit minima non odio, eveniet, 
                omnis minus  illum nostrum ullam magni sunt asperiores assumenda perferendis corporis adipisci  laudantium porro similique placeat alias`,
                pic: require('@/assets/images/about2.jpg')
              },

              {
                id: 3,
                title: "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Dignissimos iste incidunt et volupt ipsa? Alias inventore",
                desc: `
                Lorem ipsum dolor sit, amet consectetur adipisicing elit. Sit minima non odio, eveniet, omnis m illum 
                nostrum ullam magni sunt asperiores assumenda perferendis corporis adipiscilaudantium porro similique placeat
                 alias?Lorem ipsum dolor sit, amet consectetur adipisicing elit. Sit minima non odio, eveniet, 
                omnis minus  illum nostrum ullam magni sunt asperiores assumenda perferendis corporis adipisci  laudantium porro similique placeat alias`,
                pic: require('@/assets/images/about3.jpg')
              },

             
            ]
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
   .img{
    background-image: url('@/assets/images/contactus.jpg');
    background-size: cover;
   }
   
</style>
