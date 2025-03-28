<script setup>
import 'primeicons/primeicons.css';
import Card from 'primevue/card';
import { ref } from 'vue';

const count = ref(0)
const count1 = ref(0)
const count2 = ref(0)
const count3 = ref(0)
const count4 = ref(0)
const count5 = ref(0)
const count6 = ref(0)
const count7 = ref(0)
const count8 = ref(0)

</script>

<template>
    <h2>Chest Day 💪</h2>
    <span class = pin pi-user></span>
      <i class="pi pi-user" style="position: absolute; top: 20px; right: 20px; font-size: 2.0rem;"></i>
      <i class="pi pi-bell" style="position: absolute; top: 20px; left: 20px; font-size: 2.0rem;"></i>
    <Card>
        <template #title>Bench Press</template>
        <template #content>
            <p class="m-0" style="line-height: 10; font-size: 1.2rem; background-color: #444760;">
            <button style="font-size: 1.3em;"type="button" @click="count++">Reps {{ count }}</button>
            <button style="font-size: 1.3em;"type="button" @click="count1++">Reps {{ count1 }}</button>
            <button style="font-size: 1.3em;"type="button" @click="count2++">Reps {{ count2 }}</button>

            </p>
        </template>
    </Card>

    <Card>
        <template #title>Incline Press</template>
        <template #content>
            <p class="m-0" style="line-height: 10; font-size: 1.2rem; background-color: #444760;">
                <button style="font-size: 1.3em;"type="button" @click="count3++">Reps {{ count3 }}</button>
            <button style="font-size: 1.3em;"type="button" @click="count4++">Reps {{ count4 }}</button>
            <button style="font-size: 1.3em;"type="button" @click="count5++">Reps {{ count5 }}</button>
            </p>
        </template>
    </Card>
    <Card>
        <template #title>Cable Flies</template>
        <template #content>
            <p class="m-0" style="line-height: 10; font-size: 1.2rem; background-color: #444760;">
                <button style="font-size: 1.3em;"type="button" @click="count6++">Reps {{ count6 }}</button>
            <button style="font-size: 1.3em;"type="button" @click="count7++">Reps {{ count7 }}</button>
            <button style="font-size: 1.3em;"type="button" @click="count8++">Reps {{ count8 }}</button>
            </p>
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
