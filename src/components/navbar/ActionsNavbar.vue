<script setup>
import NavItem from '@/components/navbar/NavItem.vue';
    const props =defineProps({
        textColor: {
            type: String,
            default: "text-white"
        }
    })

</script>
<template>
    <nav :class="['p-3 flex items-center justify-between',textColor]">
        <h1 class="text-3xl font-bold cursor-pointer">NEWS</h1>
        <div class="flex space-x-5 items-center">
            <NavItem :textColor="textColor" title="Login" />
            <NavItem :textColor="textColor" title="Register" />
        </div>
    </nav>
</template>