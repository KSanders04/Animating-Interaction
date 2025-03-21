<script setup>
import { ref } from 'vue';
import Card from 'primevue/card';

const cards = ref([
  { id: 1, title: 'John Doe', subtitle: 'Software Engineer', content: 'Loves coding and coffee.', flipped: false },
  { id: 2, title: 'Jane Smith', subtitle: 'Designer', content: 'Passionate about designing.', flipped: false },
  { id: 3, title: 'Michael Lee', subtitle: 'Photographer', content: 'Capturing moments.', flipped: false },
  { id: 4, title: 'Lisa Brown', subtitle: 'Chef', content: 'Cooking up tasty meals.', flipped: false },
  { id: 5, title: 'David Wilson', subtitle: 'Gamer', content: 'Loves playing rocket league.', flipped: false },
  { id: 6, title: 'Emma Davis', subtitle: 'Writer', content: 'Telling good stories.', flipped: false },
  { id: 7, title: 'Chris Johnson', subtitle: 'Athlete', content: 'Loves basketball and sports.', flipped: false },
  { id: 8, title: 'Sophia Martinez', subtitle: 'Musician', content: 'Plays guitar and sings.', flipped: false }
]);

const toggleFlip = (id) => {
  const card = cards.value.find((c) => c.id === id);
  if (card) card.flipped = !card.flipped;
};
</script>

<template>
  <div class="grid-container">
    <div 
      v-for="card in cards" 
      :key="card.id" 
      class="card-wrapper" 
      @click="toggleFlip(card.id)"
    >
      <transition name="flip">
        <div class="flip-box" :class="{ flipped: card.flipped }">
          <div class="flip-box-inner">
            <div class="flip-box-front">
              <Card class="full-card">
                <template #title>{{ card.title }}</template>
                <template #subtitle>{{ card.subtitle }}</template>
                <template #content>
                  <p class="m-0">Click to flip</p>
                </template>
              </Card>
            </div>

            <div class="flip-box-back">
              <Card class="full-card">
                <template #title>Back Side</template>
                <template #content>
                  <p class="m-0">{{ card.content }}</p>
                </template>
              </Card>
            </div>
          </div>
        </div>
      </transition>
    </div>
  </div>
</template>
