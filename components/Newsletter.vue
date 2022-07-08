<template>

  <div class="">


    <div class="border border-white border-2 p-6 shadow-xl">

      <div class="w-full">
        <img :src="pic" class="mx-auto">
      </div>

      <div class="py-4 font-bold">
        {{ title }}

      </div>

      <div class="pt-2">
        {{ paragraph }}
      </div>

      <div class="pt-6 md:text-center sm:text-left lg:text-text-center xl:text-left">
        <button class="border-2 border-black text-black font-bold p-2 rounded-xl hover:text-red-500">{{ btn }}</button>
      </div>
    </div>
  </div>
</template>

<script>
import { stringify } from 'querystring';

export default {

  props: {
    title: String,
    paragraph: String,
    btn: String,
    pic: String,
  },


  
}
</script>

<style>
</style>