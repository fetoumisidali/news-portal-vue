<script setup>
    const props = defineProps({
        title:String,
        textColor:{
            type:String,
            default:"text-white"
        },
        textSize:{
            type:String,
            default:'text-base'
        }
    });
</script>

<template>
    <a :class="['hover:font-semibold', textColor,textSize ? textSize : '']" href="">{{ props.title }}</a>
</template>