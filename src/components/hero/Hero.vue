<script setup>
import ActionsNavbar from '@/components/navbar/ActionsNavbar.vue';
import TopicsNavbar from '@/components/navbar/TopicsNavbar.vue';
import HeroArticle from '@/components/hero/HeroArticle.vue';
</script>
<template>
    <section class="hero relative h-[90vh] bg-red-500 flex flex-col px-12 py-6 mb-6">
        <div class="overlay"></div>
        <div class="z-10 relative h-full w-full space-y-16">
            <div>
                <ActionsNavbar />
                <TopicsNavbar />
            </div>
            <div class="grid grid-cols-3">
                <div class="col-span-2 p-6">
                    <div class="flex items-center space-x-2 mb-6">
                        <div class="h-5 w-5 bg-red-500 rounded-full"></div>
                        <h1 class="text-white text-xl font-light">Hot Topic</h1>
                    </div>
                    <HeroArticle/>
                </div>
                <div class="col-span-1">

                </div>
            </div>
        </div>
    </section>
</template>
<style scoped>
.hero {
    background-size: cover;
    background-image: url('/images/hero-background.jpg');
    background-position: center;
}

.overlay {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-color: rgba(0, 0, 0, 0.6);
    /* Adjust opacity as needed */
    z-index: 1;
}
</style>