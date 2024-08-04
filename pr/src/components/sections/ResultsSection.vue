<template>
    <div class="h-screen text-center py-20 px-20 flex" id="results">
        Our Results
        <div class="w-1/3 h-4/5 " id="map"></div>
    </div>
</template>

<script setup>
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