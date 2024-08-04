<template>
    <section class=" px-12 gap-16 justify-center h-screen flex text-center pt-32 bg-[#142242]" id="contact">


        <div class="card flex flex-col w-1/3 items-center gap-24 ">
            <div class="text-lg">
                <h1 class="text-3xl">Lorem ipsum dolor sit amet consectetur adipisicing elit!</h1>
            </div>
            <Accordion class="w-full" value="0">
                <AccordionPanel value="0">
                    <AccordionHeader>Header I</AccordionHeader>
                    <AccordionContent>
                        <p class="m-0">
                            Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut
                            labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco
                        </p>
                    </AccordionContent>
                </AccordionPanel>
                <AccordionPanel value="1">
                    <AccordionHeader>Header II</AccordionHeader>
                    <AccordionContent>
                        <p class="m-0">
                            Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque
                            laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi
                        </p>
                    </AccordionContent>
                </AccordionPanel>
                <AccordionPanel value="2">
                    <AccordionHeader>Header III</AccordionHeader>
                    <AccordionContent>
                        <p class="m-0">
                            At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis praesentium
                            voluptatum deleniti atque corrupti quos dolores et quas molestias excepturi sint occaecati

                        </p>
                    </AccordionContent>
                </AccordionPanel>
            </Accordion>
        </div>
        <div class="w-1/3 h-4/5 " id="map"></div>


    </section>


</template>

<script setup>

import Accordion from 'primevue/accordion';
import AccordionPanel from 'primevue/accordionpanel';
import AccordionHeader from 'primevue/accordionheader';
import AccordionContent from 'primevue/accordioncontent';


import { ref, onMounted } from 'vue';
import "leaflet/dist/leaflet.css";
import * as L from 'leaflet';

const initialMap = ref(null);

onMounted(() => {
    initialMap.value = L.map('map').setView([41.263767043474765, 69.16254061842835], 20);
    L.tileLayer('https://tile.openstreetmap.org/{z}/{x}/{y}.png', {
        maxZoom: 19,
        attribution: '&copy; <a href="http://www.openstreetmap.org/copyright">OpenStreetMap</a>'
    }).addTo(initialMap.value);
});
</script>