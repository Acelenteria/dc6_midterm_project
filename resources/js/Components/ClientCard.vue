<template>

    <div class='flex items-center justify-center py-5 px-2' :class="themeMode">
        <div class='w-full max-w-md  mx-auto  rounded-3xl shadow-xl overflow-hidden'>
            <div class='max-w-md mx-auto'>
            <!-- <div class='h-[236px]' style='background-image:url(https://img.freepik.com/free-photo/pasta-spaghetti-with-shrimps-sauce_1220-5072.jpg?w=2000&t=st=1678041911~exp=1678042511~hmac=e4aa55e70f8c231d4d23832a611004f86eeb3b6ca067b3fa0c374ac78fe7aba6);background-size:cover;background-position:center'>
            </div> -->
            <div class='p-4 sm:p-6'>
                <p class='font-bold text-[20px] leading-7 mb-1'>{{ client.last_name }} , {{ client.first_name }}</p>
                <div class='flex flex-row'>
                    <p class='text-[15px] font-bold'>{{ client.address }}</p>

                </div>
                <p class=' font-[15px] mt-4'>Phone number{{client.phone }}</p>
                <p class='font-[15px] '>Credit limit: {{ client.credit_limit }}</p>


                <button style="background-color:#FFC0CB" @click="open(client)" class='block mt-10 w-full px-4 py-3 font-medium tracking-wide text-center capitalize transition-colors duration-300 transform rounded-[14px] focus:outline-none focus:ring focus:ring-teal-300 focus:ring-opacity-80'>
                    View on Client
                </button>

            </div>
            </div>
        </div>
    </div>



</template>

<script setup>
import { router } from '@inertiajs/vue3';
import { inject } from 'vue';

const props = defineProps({
    client: Object
})

function open(client) {
    router.visit('/clients/' + client.id)
}

const themeMode = inject('themeMode')



</script>
