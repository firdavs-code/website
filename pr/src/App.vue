<template>
    <div class="">
        <AppHeader></AppHeader>
        <main class="scroll-smooth ">
            <MainSection></MainSection>
            <AboutSection></AboutSection>

            <section class="h-screen py-20 px-32 flex justify-between bg-[#142242] " id="teachers">
                <img class=" rounded-2xl" src="./assets/photos/b.jpg">
                <div class="">
                    <h1 class="text-3xl font-bold text-orange-500 gap-10  flex">Al-Xorazmiy academiyasi asoschisi</h1>

                    <h2 class="text-gray-300 italic text-xl py-10  ">" Dunyoda minglab o’zbek yoshlariga qo’l mehnati emas,
                        yuqori
                        <br> intellekti uchun haq
                        to’lansa, millionlab yoshlar o'z oilalaridagi<br> moliyaviy ahvolni o'nglab, chet elda
                        qiynalib ishlayotgan yaqinlarini<br> vatanga qaytishiga sababchi bo’lsa va dunyoni yaxshi
                        tarafga<br> o’zgartiruvchi qarorlar qabul qiladigan, gigant kompaniyalarning<br> boshqaruv
                        pozitsiyasini egallaydigan mutaxassislarni yetishtira olsak,<br> o'z oldimizga qo'ygan
                        maqsadlarimizga erishgan bo'lamiz. "
                    </h2>
                    <h3 class="text-3xl gap-10 font-bold text-gray-300  ">Al-Xorazmiy academiyasi asoschisi</h3>
                    <h4 class="text-xl py-4 gap-10 font-mono text-orange-500">Alisher Uzakov</h4>
                </div>

            </section>



            <section class="h-screen text-center py-20" id="contact">Contact</section>
        </main>
    </div>
</template>

<script setup>
import AppHeader from './components/AppHeader.vue';
import MainSection from './components/sections/MainSection.vue';
import AboutSection from './components/sections/AboutSection.vue';
</script>