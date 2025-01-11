<script setup>
const props = defineProps({
    isRow: {
        type: Boolean,
        default: false
    }
})
</script>


<template>
    <div class="p-6 bg-gray-100 rounded-lg flex" :class="{ 'flex-row space-x-6': isRow, 'flex-col': !isRow }">
        <img src="/images/fire.jpg" class="rounded-xl" :class="{ 'w-80': isRow }">
        <div>
            <h2 class="text-2xl font-bold mt-6">California infernos in January? Why wildfire season keeps
                getting longer and more devastating.</h2>
            <p class="mt-3 text-gray-800">Lorem ipsum dolor sit amet consectetur, adipisicing elit. Voluptatibus
                fugiat delectus eius officiis doloremque, enim quibusdam quae doloribus laborum dolorem ducimus
                amet assumenda soluta id nihil accusamus mollitia modi omnis.</p>
            <a href="" class="inline-block text-xl font-normal text-white bg-black mt-4 px-6 py-3 rounded-full">Read
                More</a>
        </div>
    </div>
</template>