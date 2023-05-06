<template>
  <h1>hello this is product page</h1>
  <NuxtLink :to="'/products'" :active-class="'active'">product</NuxtLink>
</template>

<script lang="ts" setup>
console.log("hello world!");
</script>
