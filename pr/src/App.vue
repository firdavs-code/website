<template>
    <div class="">
        <AppHeader></AppHeader>
        <main class="scroll-smooth ">
            <MainSection></MainSection>
            <AboutSection></AboutSection>
            <FounderSection></FounderSection>
            <ContactSection></ContactSection>
        </main>
    </div>
</template>

<script setup>
import AppHeader from './components/AppHeader.vue';
import MainSection from './components/sections/MainSection.vue';
import AboutSection from './components/sections/AboutSection.vue';
import FounderSection from './components/sections/FounderSection.vue';
import ContactSection from './components/sections/ContactSection.vue';



</script>