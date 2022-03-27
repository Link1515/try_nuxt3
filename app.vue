<template>
  <div>
    <!-- <NuxtWelcome /> -->
    <NuxtPage />

    <h2>store</h2>
    <p>{{ store.count }}</p>
    <button @click="store.count++">++</button>
  </div>
</template>

<script setup>
import { useStore } from './stores/conter.ts';

const { $hello } = useNuxtApp();
console.log($hello());

const store = useStore();
</script>
