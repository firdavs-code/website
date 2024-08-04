<template>
  <div class="fixed w-full z-50">
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
