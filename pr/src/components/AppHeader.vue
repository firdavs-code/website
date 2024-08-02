<template>
  <!-- <header class="flex justify-between fixed bg-opacity-90 top-0 py-4 px-10 w-full
     bg-orange-500 items-center text-white">
    <h1 class="text-2xl ">Al-Khorezmi</h1>
    <nav class="flex gap-8 font-sans">
      <a href="#main">Main</a>
      <a href="#about">About us</a>
      <a href="#teachers">Teachers</a>
      <a href="#contact">Contact</a>
    </nav>
    <div>
      <a href="tel:977775577" class="border p-2 rounded-2xl bg-[#142242]">+998 (98) 777-77-77</a>
    </div>
  </header> -->
  <div class="fixed w-full">
    <Menubar  :model="items" >

      <template #end>
        <h1 class="text-2xl  ">Al-Khorezmi</h1>
      </template>
    </Menubar>
  </div>
</template>


<script setup>
import Menubar from "primevue/menubar";
import { ref } from "vue";


const items = ref([
  {
    label: 'Main',
    icon: 'pi pi-home',
    url: '#main'
  },
  {
    label: 'Courses',
    icon: 'pi pi-book',
    url: '#courses'
  },
  {
    label: 'Founder',
    icon: 'pi pi-user',
    url: '#teachers'
  },
  {
    label: 'Results',
    icon: 'pi pi-info-circle',
    url: '#results'
  },
  {
    label: 'Contact',
    icon: 'pi pi-envelope',
    url: '#contact'
  }
]);
</script>
