<script setup>
import AuthenticatedLayout from '@/Layouts/AuthenticatedLayout.vue';
import {Head} from '@inertiajs/vue3'
</script>

<template>
    <Head title="Edit client"/>

    <AuthenticatedLayout>
        <template #header>
            <h2 class="font-semibold text-xl  leading-tight">
                Edit Client
            </h2>
        </template>
        <!-- component -->
        <div class="py-12">
            <div class="max-w-5xl mx-auto sm:px-6 lg:px-8">
                <div class="bg-white shadow-md rounded px-8 pt-6 pb-8 mb-4 flex flex-col my-2">
                    <form>
                        <div class="grid gap-6 mb-6 lg:grid-cols-2">
                            <div>
                                <label for="first_name" class="block mb-2 text-sm font-medium text-black dark:text-white-300">Name</label>
                                <input type="text" id="first_name" class="bg-gray-50 border border-gray-300 text-black text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5  dark:focus:ring-blue-500 dark:focus:border-blue-500" placeholder="John" >
                            </div>
                            <div>
                                <label for="email" class="block mb-2 text-sm font-medium text-black ">Email</label>
                                <input type="email" id="email" class="bg-gray-50 border border-gray-300 text-black text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5  dark:focus:ring-blue-500 dark:focus:border-blue-500" placeholder="Doe@example.com" >
                            </div>
                            <div>
                                <label for="address" class="block mb-2 text-sm font-medium text-black ">Address</label>
                                <input type="text" id="address" class="bg-gray-50 border border-gray-300 text-black text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5  dark:placeholder-gray-400 dark:focus:ring-blue-500 dark:focus:border-blue-500" placeholder="Address" >
                            </div>
                            <div></div>
                            <div>
                                <label for="password" class="block mb-2 text-sm font-medium text-black ">Password</label>
                                <input type="password" id="password" class="bg-gray-50 border border-gray-300 text-black text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5  dark:focus:ring-blue-500 dark:focus:border-blue-500" placeholder="*******" >
                            </div>
                            <div>
                                <label for="confirmPassword" class="block mb-2 text-sm font-medium text-black ">Confirm Password</label>
                                <input type="password" id="confirmPassword" class="bg-gray-50 border border-gray-300 text-black text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5  dark:focus:ring-blue-500 dark:focus:border-blue-500" placeholder="*******" >
                            </div>

                            </div>
                            <div class="flex justify-between mt-5">
                                <h1 class="text-3xl font-medium text-gray-700 "></h1>
                                <button type="submit" class="text-white bg-blue-700 hover:bg-blue-800 focus:ring-4 focus:outline-none focus:ring-blue-300 font-medium rounded-lg text-sm w-full sm:w-auto px-5 py-2.5 text-center dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800">Update user</button>
                            </div>

                    </form>
                </div>
            </div>
         </div>
    </AuthenticatedLayout>
</template>
