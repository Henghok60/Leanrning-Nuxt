<template>
  <div>
    <div class="flex">
      <div class="sidebar bg-slate-700 w-1/6 top-0 bottom-0 h-screen">
        <div class="p-3 bg-white"><h1 class="font-bold">POS</h1></div>
        <div
          v-for="item in navItem"
          class="hover:bg-slate-300 p-2"
          :key="item.label">
          <NuxtLink :to="item.link">
            <h1>{{ item.label }}</h1>
          </NuxtLink>
        </div>
      </div>
      <div class="w-full">
        <div class="p-3 bg-slate-300"><h1 class="font-bold">POS</h1></div>
        <div class="m-4">
          <slot />
        </div>
      </div>
    </div>
  </div>
</template>
<script lang="ts" setup>
const navItem = [
  {
    label: "Dashboard",
    link: "/",
    hasChild: false,
  },
  {
    label: "Product",
    link: "/products",
    hasChild: false,
  },
  {
    label: "Category",
    link: "/categories",
    hasChild: false,
  },
];
</script>
<style></style>
