<template>

    <div class="my-10 border-b border-gray-300 flex justify-between items-center">
        <div>
            <div class="text-2xl">{{ title }}</div>
            <div class="">{{ desc }}</div>
        </div>

        <div>
            <button @click="handleShowWhenClicked(title, desc)" class="px-3 py-2 bg-gray-600 text-white rounded-full text-sm">Show</button>
        </div>
    </div>




</template>


<script>

export default {

    props: {
        title: String,
        desc: String,
    },

    methods: {
        handleShowWhenClicked(title, desc){

            let my_data = {
                title: title,
                desc: desc
            }
            
            this.$emit("showButtonClicked", my_data)
        }
    }

}

</script>