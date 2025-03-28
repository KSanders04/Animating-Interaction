<script setup>
import 'primeicons/primeicons.css';
import Card from 'primevue/card';
import { ref } from 'vue';

const value = ref(null)

</script>

<template>
    <h3>How was your Workout?</h3>
    <span class = pin pi-user></span>
      <i class="pi pi-user" style="position: absolute; top: 20px; right: 20px; font-size: 2.0rem;"></i>
      <i class="pi pi-bell" style="position: absolute; top: 20px; left: 20px; font-size: 2.0rem;"></i>
    <Card>
        <template #title>Rate ⭐</template>
        <template #content>
            <p class="m-0" style="line-height: 5; font-size: 1.2rem; background-color: #444760;">
                ⭐⭐⭐⭐⭐
            </p>
        </template>
    </Card>

    <Card>
        <template #title>Additional Info</template>
        <template #content>
        </template>
    </Card>
    <div class="card">
      <a href="Review.vue" class="button" style="text-decoration: none; color: white; background-color: #444760; padding: 10px 20px; border-radius: 5px; font-size: 1.5rem;">Done!</a>
  </div>
  </template>

<style scoped>
:deep(.p-card-title) {
  background-color: #444760;
  font-size: 1.9rem;
  padding: px;
  border-radius: 5px;
}
</style>
