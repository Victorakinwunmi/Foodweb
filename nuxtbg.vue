<div class="bg-no-repeat bg-cover bg-center" :style="{backgroundRepeat: 'no-repeat' + ';' , backgroundImage: 'url(' + require('@/assets/images/hmc_banner.jpeg') +')'}">
</div>

<!-- greetings.vue example -->

 <Greetings :full_name="reactive_full_name" />

    {{reactive_full_name}}

    <input v-model="reactive_full_name" />

<!-- Put this into data of ur index -->
  reactive_full_name: "",