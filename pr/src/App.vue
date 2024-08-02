<template>
    <div class="">
        <AppHeader></AppHeader>
        <main class="scroll-smooth ">
            <MainSection></MainSection>
            <CoursesSection></CoursesSection>
            <FounderSection></FounderSection>
            <ResultsSection></ResultsSection>
            <ContactSection></ContactSection>
        </main>
    </div>
</template>

<script setup>
import AppHeader from './components/AppHeader.vue';
import MainSection from './components/sections/MainSection.vue';
import FounderSection from './components/sections/FounderSection.vue';
import ContactSection from './components/sections/ContactSection.vue';
import CoursesSection from './components/sections/CoursesSection.vue';
import ResultsSection from './components/sections/ResultsSection.vue';



</script>