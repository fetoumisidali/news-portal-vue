<script setup>
import SectionTitle from '@/components/sections/SectionTitle.vue';
import LatestArticles from '../articles/LatestArticles.vue';


</script>

<template>
    <section class="flex flex-col">
        <SectionTitle title="Latest" />
        <div class="grid grid-cols-3 gap-6 mx-12 my-6">
            <div class="col-span-1">
                <LatestArticles />
            </div>
            <div class="col-span-2 space-y-6">
                <LatestArticles :isRow="true" />
                <LatestArticles :isRow="true" />
            </div>
        </div>
    </section>
</template>