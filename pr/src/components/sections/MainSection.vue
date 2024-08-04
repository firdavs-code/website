<template>
    <section class="h-screen flex flex-col items-center justify-center pt-10 px-20 gap-8 bg-[#142242]" id="main">
        <h1 class="text-5xl mon-400 font-bold text-white">
            Xorazmiy Imzo Academiyasiga</h1>
        <div class="items-start gap-8 flex">
            <div class="gap-10 flex flex-col ">
                  <p class="text-2xl font-medium text-white leading-relaxed w-fit  text-justify  ">
                Bizning academiyada hozida ingiliz tili, SAT, Matematika, hamda boshqa koplab xususiy
                maktablardan prizident, Al-Xorazmiy kabi maktablarg hamda, xususiy universitetlarga kirishga
                yordam beradi. Akademiyamizda oz kasbning mutahasislari dars berib boradi!
            </p>
            <Button as="a" icon="pi pi-phone" class="w-fit " href="tel:+998977777777" label="(998) 97-777-77-77" severity="success"/>
            </div>
            <img class=" rounded-2xl" src="@/assets/photos/d.jpeg">
        </div>
    </section>
</template>

<script setup>
import Button from 'primevue/button';
</script>