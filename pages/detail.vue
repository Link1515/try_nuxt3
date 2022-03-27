<template>
  <div>
    <h2>detail page</h2>
    <h3>counter</h3>
    {{ counter }}
  </div>
</template>

<script setup>
const counter = useCounter();
</script>
