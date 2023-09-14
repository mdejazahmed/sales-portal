<template>
  <v-layout class="rounded rounded-md">
    
    <Navbar/>
    <v-main class="d-flex align-center justify-center" style="min-height: 300px;">
      <router-view/>
    </v-main>
  </v-layout>
</template>

<script setup>
import Navbar from '@/components/Navbar.vue';


</script>
