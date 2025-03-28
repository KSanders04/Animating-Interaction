<script setup>
import HomePage from './components/HomePage.vue'
import 'primeicons/primeicons.css';
</script>

<template>
    <h1>IronTrack - Fitness Planner</h1>
    <span class = pin pi-user></span>
      <i class="pi pi-user" style="position: absolute; top: 20px; right: 20px; font-size: 2.0rem;"></i>
      <i class="pi pi-bell" style="position: absolute; top: 20px; left: 20px; font-size: 2.0rem;"></i>

    <div>
    <a>
      <img src="./assets/Workingout.webp" alt="Workout" height="456" width="271" style="border-radius: 50px;"/>
    </a>
  </div>
  <HomePage/>
</template>