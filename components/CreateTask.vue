<template>
<div>
    <div class="text-center text-xl mb-4 font-semibold text-gray-500">
      {{desc}}
    </div>

  <div class="w-full">
     <form action="" class="mx-0 md:mx-28">
       <input type="text" placeholder="Title" class="p-4 w-full outline-none">
       <input type="time" placeholder="Time" class="p-4 outline-none">
    
     </form>

    <div class="flex justify-end">
        <button class="text-gray-black p-2 mt-16 rounded-lg border border-black">{{btn}}</button>
    </div>
  </div>
   

</div>
 
   
</template>

<script>

export default{
  props: {
       title: String,
       desc: String,
       btn: String,
    },

}
</script>

<style>

</style>