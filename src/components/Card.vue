<script setup>
defineProps(["card"])
</script>

<template>
    <div class="shadow hover:shadow-md hover:scale-105 transition cursor-pointer">
        <img :src="`/images/${card}.png`">
        <div class="bg-white p-4">
            <h3 class="capitalize font-semibold">{{ card }}</h3>
            <p class="text-sm text-gray-400">10km from you</p>
        </div>
    </div>
</template>