<script setup>
import { ref } from 'vue'
import Workout from './Workout.vue';

defineProps({
  msg: String,
})

</script>

<template>
  <div class="card">
      <a href="Workout.vue" class="button" style="text-decoration: none; color: black; background-color: white; padding: 10px 20px; border-radius: 5px; font-size: 2rem;">Start Workout</a>
  </div>
</template>
