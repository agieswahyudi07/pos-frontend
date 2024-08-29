<script setup>
import { ref } from 'vue';
const username = ref('')
const password = ref('')
const rememberMe = ref('')
</script>
<template>
    <div class="flex items-center justify-center min-h-dvh bg-white">
        <div class="z-10 border rounded-md px-10 pb-5 bg-white shadow-md">
            <h1 class="flex justify-center text-xl font-medium text-black my-5">Login</h1>
            <div class="space-y-3">
                <input class="w-full border border-gray-500 rounded-md flex justify-center text-center placeholder:text-sm placeholder:text-center " v-model="username" type="text" placeholder="username">
                <input class="w-full border border-gray-500 rounded-md flex justify-center text-center placeholder:text-sm placeholder:text-center" v-model="password" type="password" placeholder="password">
                <div class="flex justify-content-start">
                    <input class="" v-model="rememberMe" type="checkbox">
                    <p class=" text-sm pb-1 pl-1">remember me</p>
                </div>
            </div>
            <p class="flex justify-center text-sm pt-4">don't have any account ? <a class=" pl-1 font-bold text-blue-600 hover:text-blue-500" href="">register here</a></p>
        </div>
    </div>
</template>
