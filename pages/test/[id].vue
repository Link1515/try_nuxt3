<template>
  <div>
    <h2>test/[id] page</h2>
    <p>{{ $route.params.id }}</p>
    <NuxtLink to="/">back to home</NuxtLink>
  </div>
</template>
