<template>



    <div class="" id="grids">
        <div class="group bg-no-repeat bg-cover bg-center h-80 mr-4 mb-4 shadow-xl"
            :style="{ backgroundRepeat: 'no-repeat' + ';', backgroundImage: 'url(' + pic + ')' }">
            <div>
             <div class="group-hover:opacity-100 duration-500 transition ease-in-out  opacity-0 p-10 text-white bg-black bg-opacity-80 w-full h-80 ">
                <div class="Font-bold text-4xl ">
                   <div class="font-mono mt-10">{{desc}}</div>
                </div>
                <div class="mt-10">
                   <button class="border bg-green-700 rounded-full py-2 px-6 font-bold">{{btn}}</button>
                </div>
             </div>
            </div>
        </div>

    </div>

    

</template>

<script>

export default {

    props: {
        pic: String,
        desc: String,
        btn: String,
    },



}
</script>

<style>

</style>