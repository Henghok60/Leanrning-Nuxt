<template>
  <h1>hello this is product page</h1>
  <NuxtLink :to="'/products'">product</NuxtLink>
</template>
<script lang="ts" setup>
definePageMeta({
  layout: "default-layout",
});
</script>
