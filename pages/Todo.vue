<template>
<div>
   <div class="flex">
     <div class="w-1/12 bg-gray-300">
        <img :src="require('@/assets/images/Logo.png')" class="my-6">
     </div>

        <div class="w-11/12 bg-gray-200">

            <div class="w-full mt-6">
                <button :class="is_revealed ? 'hidden' : 'block' " class=" mx-6 border rounded-md bg-white p-4 font-semibold" @click="ShowForm">Add task</button>
            </div>
            
            <div class="px-24 py-14">
              <div v-for="item in todos" :key="item.id">
                <div class="flex justify-between bg-white rounded-lg w-full p-6 my-6">
                  <div>
                    <h1 class="font-medium text-lg">{{item.title}}</h1>
                    <p class="mt-3 text-base">{{item.time}}</p>
                  </div>
                  <button>Delete</button>
                </div>

              </div>
            </div>

          
            
              <div :class="is_revealed ? 'block' : 'hidden' " class="bg-black bg-opacity-30 absolute top-0 right-0 left-0 h-screen">
                
                  <div  class="bg-white rounded-2xl mt-40 p-6 mx-10 md:mx-28 shadow-xl">

                    <div class="w-full mt-6 flex justify-end">
                      <button :class="is_revealed ? 'flex' : 'hidden' " class=" mx-6 text-red-500 p-4 font-semibold" @click="HideForm">Cancel</button>
                    </div>

                    <CreateTask
                      title=""
                      desc="Kindly input the title and time"
                      btn="Create task">

                        

                    </CreateTask>
                              
                  </div>
              </div>


          
            
        </div>  
   </div>



</div>
</template>

<script>
import CreateTask from '../components/CreateTask.vue';

export default{
    components: { CreateTask },

    data() {

       return {
        is_revealed: false,
       

        todos: [
          {
            id: 1,
            title: "Go to a friend's house",
            time: "12:00 am",
          },

          {
            id: 2,
            title: "Clean the house",
            time: "01:00 pm",
          },

          {
            id: 3,
            title: "Office cleaning",
            time: "04:30 am",
          },

          {
            id: 4,
            title: "Try to apply for jobs",
            time: "11:00 pm",
          },

          {
            id: 5,
            title: "Post on instagram",
            time: "07:15 pm",
          },
        ]
      }
    },

     methods: {
        ShowForm() {
            this.is_revealed = true;
        },
        HideForm() {
            this.is_revealed = false;
        }
    },

}
</script>

<style>

</style>