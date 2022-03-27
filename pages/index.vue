<template>
  <div>
    <!-- <Header></Header>
    <BaseBtnsMyComp></BaseBtnsMyComp> -->
    <h1>Index Page</h1>
    <NuxtLink to="/detail">Detail Page</NuxtLink> | <NuxtLink to="/user-admin/1">admin Page</NuxtLink> |
    <NuxtLink to="/test">test page without params</NuxtLink> |
    <NuxtLink to="/test/123">test page with params</NuxtLink> |

    <h2>to-do</h2>
    <div v-for="todo in todos" :key="todo.id">
      <input type="checkbox" v-model="todo.complete" />
      <strong>{{ todo.title }}</strong>
    </div>

    <h2>counter</h2>
    <p>
      {{ counter }}
    </p>
    <button @click="counter++">counter++</button>
  </div>
</template>

<script setup>
// const { data: todos } = await useAsyncData('todos', () => $fetch('/api/todo'));
const { data: todos } = await useFetch('/api/todo');
console.log(todos);
console.log(process.server);
console.log(process.client);

const counter = useCounter();
</script>
