<template>
    <div class="">
        <AppHeader></AppHeader>
        <main class="scroll-smooth ">
            <MainSection></MainSection>
            <section class="h-screen text-center py-20" id="about">
                <div class="text-stone-500 text-3xl pb-10">
                    <h1>Al-Xorazmiynig yonalishlari</h1>
                </div>
                <div class="flex justify-between">
                    <p class="text-stone-500 w-1/2 py-2 px-10 text-xl italic">
                        Bizning academiyada hozida ingiliz tili, SAT, <br>Matematika,hamda boshqa koplab xususiy
                        maktablardan prizident,Al-Xorazmiy kabi maktablarg hamda,<br>xususiy universitetlarga kirishga
                        yordam
                        beradi.<br>Academiyamizda oz kasbning ,utahasislari dars berib boradi
                    </p>
                    <img class="size-2/5 rounded-xl" src="./assets/photos/c.jpg">

                </div>

            </section>

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
</script>