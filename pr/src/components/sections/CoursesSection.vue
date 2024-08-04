<template>
    <div class="h-screen text-center py-20" id="courses">
        <div class="card">
            <Carousel :value="products" :numVisible="4" :numScroll="1" :responsiveOptions="responsiveOptions"
                :autoplayInterval="3000">
                <template #item="slotProps">
                    <Card style="width: 25rem; overflow: hidden; border-radius: 20px">
                        <template #header>
                            <img alt="user header" src="https://primefaces.org/cdn/primevue/images/usercard.png" />
                        </template>
                        <template #title>{{ slotProps.data.name }}</template>
                        <template #subtitle>{{ slotProps.data.teacher + ' - ' + slotProps.data.students + ' bitiruvchi'}}</template>
                        <template #content>
                            <p class="m-0 leading-relaxed text-justify max-h-12">
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


const products = ref([
    {
        id: '1000',
        name: 'Math',
        teacher: "Jhon Doe",
        description: 'Eng zor matematika kursida oqing. Biz bila DTM dan maximum ball olin va eng zor oliygohlarga kiring!',
        image: 'bamboo-watch.jpg',
        price: 50,
        students: 5
    },
    {
        id: '1001',
        name: 'Fizika',
        teacher: "Jhon Doe",
        description: 'Eng zor Fizika kursida oqing. Biz bila DTM dan maximum ball olin va eng zor oliygohlarga kiring!',
        image: 'bamboo-watch.jpg',
        price: 650,
        students: 5
    },
    {
        id: '1002',
        name: 'Ingliz tili',
        teacher: "Jhon Doe",
        description: 'Eng zor Ingliz tili kursida oqing. Biz bila DTM dan maximum ball olin va eng zor oliygohlarga kiring!',
        image: 'bamboo-watch.jpg',
        price: 605,
        students: 5
    },
    {
        id: '1003',
        name: 'IELTS',
        teacher: "Ahror Xalilov",
        description: 'Eng zor IELTS kursida oqing. Biz bila DTM dan maximum ball olin va eng zor oliygohlarga kiring!',
        image: 'bamboo-watch.jpg',
        price: 405,
        students: 5
    },
    {
        id: '1004',
        name: 'SAT',
        teacher: "Jhon Doe",
        description: 'Eng zor SAT kursida oqing. Biz bila DTM dan maximum ball olin va eng zor oliygohlarga kiring!',
        image: 'bamboo-watch.jpg',
        price: 650,
        students: 5
    },
    {
        id: '1005',
        name: 'GMAT',
        teacher: "Jhon Doe",
        description: 'Eng zor GMAT kursida oqing. Biz bila DTM dan maximum ball olin va eng zor oliygohlarga kiring!',
        image: 'bamboo-watch.jpg',
        price: 600,
        students: 5
    },
    {
        id: '1006',
        name: 'TOEFL',
        teacher: "Jhon Doe",
        description: 'Eng zor TOEFL kursida oqing. Biz bila DTM dan maximum ball olin va eng zor oliygohlarga kiring!',
        image: 'bamboo-watch.jpg',
        price: 300,
        students: 5
    }
]);
const responsiveOptions = ref([
    {
        breakpoint: '1400px',
        numVisible: 3,
        numScroll: 1
    },
    {
        breakpoint: '1199px',
        numVisible: 2,
        numScroll: 1
    },
    {
        breakpoint: '767px',
        numVisible: 2,
        numScroll: 1
    },
    {
        breakpoint: '575px',
        numVisible: 1,
        numScroll: 1
    }
]);

</script>

