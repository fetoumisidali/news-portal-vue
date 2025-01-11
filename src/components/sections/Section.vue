<script setup>
    import SectionTitle from './SectionTitle.vue';
import SectionArticle from '@/components/sections/SectionArticle.vue';
    const props = defineProps({
        title:String
    })
</script>
<template>
    <section class="flex flex-col">
        <SectionTitle :title="title" />
        <div class="grid grid-cols-3 gap-6 mx-12 my-6">
            <SectionArticle />
            <SectionArticle />
            <SectionArticle />
        </div>
    </section>
</template>

