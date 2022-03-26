<template>
  <div>
    <Header></Header>
    <BaseBtnsMyComp></BaseBtnsMyComp>
    <h1>Index Page</h1>
    <NuxtLink to="/detail">Detail Page</NuxtLink> | <NuxtLink to="/user-admin/1">admin Page</NuxtLink> |
    <NuxtLink to="/test">test page without params</NuxtLink> |
    <NuxtLink to="/test/123">test page with params</NuxtLink> |
  </div>
</template>
