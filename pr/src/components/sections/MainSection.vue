<template>
    <section class="h-screen flex flex-col items-center justify-center pt-10 px-20 gap-16 bg-[#142242]" id="main">
        <h1 class="text-6xl mon-400 font-bold text-white">
            Al Xorazmiy Imzo Academiyasi</h1>
        <div class="items-start gap-8 flex justify-center">
            <div class="gap-10 flex flex-col w-1/2">
                <p class="text-2xl font-medium text-white leading-relaxed text-justify  ">
                    Bizning academiyada hozirda ingiliz tili, SAT, Matematika tayolanishingiz mumkin. Hamda koplab
                    xususiy Prezident, Al-Xorazmiy, Beruni kabi maktablarga hamda, va universitetlarga kirishga
                    yordam beradi. Akademiyamizda oz kasbning mutahasislari dars berib boradi. Biz bilan ilm oling!
                </p>
                <Button as="a" icon="pi pi-phone" class="w-fit " href="tel:+998977777777" label="(998) 97-777-77-77"
                    severity="success" />
            </div>
            <img class=" rounded-2xl" src="@/assets/photos/d.jpeg">
        </div>
    </section>
</template>

<script setup>
import Button from 'primevue/button';
</script>