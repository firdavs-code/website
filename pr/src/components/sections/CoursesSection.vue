<template>
    <div class="h-screen text-center py-20 justify-center flex flex-col" id="courses">
        <h1 class="text-4xl font-medium"> Bizning Kurslar</h1>
        <div class="card     text-white">
            <h3 class="text-2xl font-medium">Bizning akademiyada kurslar 3 oydan boshlab 2 yilgacha</h3>
            <Carousel :value="courses" :numVisible="4" :numScroll="1" :responsiveOptions="responsiveOptions"
                :autoplayInterval="3000">
                <template #item="slotProps">
                    <Card style="width: 24rem; overflow: hidden; border-radius: 20px; margin-left: auto; margin-right: auto">
                        <template #header>
                            <img alt="user header" src="https://primefaces.org/cdn/primevue/images/usercard.png" />
                        </template>
                        <template #title>{{ slotProps.data.name }}</template>
                        <template #subtitle>{{ slotProps.data.teacher + ' - ' + slotProps.data.students + ' bitiruvchi'}}</template>
                        <template #content>
                            <p class="m-0 text-justify min-h-16 max-h-18">
                                {{ slotProps.data.description }}
                            </p>
                        </template>
                        <template #footer>
                            <div class="flex gap-4 mt-0">
                                <Button :label="'Oyiga atiga ' + slotProps.data.price + ' ming so\'m'" class="w-full" />
                            </div>
                        </template>
                    </Card>
                </template>
            </Carousel>
        </div>
    </div>
</template>

<script setup>
import { ref } from "vue";
import Carousel from 'primevue/carousel';
import Card from 'primevue/card';
import Button from 'primevue/button';
import { courses } from '@/data/courses';

const responsiveOptions = ref([
    {
        breakpoint: '1550px',
        numVisible: 3,
        numScroll: 1
    },
    {
        breakpoint: '1200px',
        numVisible: 2,
        numScroll: 1
    },
    {
        breakpoint: '767px',
        numVisible: 2,
        numScroll: 1
    },
    {
        breakpoint: '855px',
        numVisible: 1,
        numScroll: 1
    }
]);

</script>

