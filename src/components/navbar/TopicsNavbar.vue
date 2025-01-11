<script setup>
import NavItem from '@/components/navbar/NavItem.vue';
const props = defineProps({
    textColor: {
        type: String,
        default: "text-white"
    }
})

</script>
<template>
    <nav :class="['p-3 flex items-center space-x-20 justify-center', textColor]">
        <NavItem :textColor="textColor" textSize="text-xl" title="Sport" />
        <NavItem :textColor="textColor" textSize="text-xl" title=" Health" />
        <NavItem :textColor="textColor" textSize="text-xl" title=" Political" />
        <NavItem :textColor="textColor" textSize="text-xl" title="Finance" />
        <NavItem :textColor="textColor" textSize="text-xl" title="Life" />
    </nav>
</template>