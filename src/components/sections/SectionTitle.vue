<script setup>
    const props = defineProps({
        title:String
    })
</script>

<template>
    <div class="flex px-12 py-3 justify-between items-center">
        <h1 class="text-4xl font-medium">{{ props.title }}</h1>
        <a href="" class="text-white bg-red-500 px-6 py-2 rounded-full hover:bg-red-600">View All</a>
    </div>
</template>