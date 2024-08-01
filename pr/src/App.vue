<template>
    <div class="">
        <AppHeader></AppHeader>
        <main class="scroll-smooth ">
            <MainSection></MainSection>
            <AboutSection></AboutSection>
            <FounderSection></FounderSection>
            <section class="h-screen text-center py-20" id="contact">Contact</section>
        </main>
    </div>
</template>

<script setup>
import AppHeader from './components/AppHeader.vue';
import MainSection from './components/sections/MainSection.vue';
import AboutSection from './components/sections/AboutSection.vue';
import FounderSection from './components/sections/FounderSection.vue';
</script>