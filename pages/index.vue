<template>
  <section class="p-4 flex justify-center min-h-[100svh]">
    <NuxtLink to="/introduction">introduction</NuxtLink>
  </section>
</template>

<script setup>
useHead({
  title: "Introduction",
});
</script>

<style scoped>
p,
li {
  @apply dark:text-[#d1d5db];
}
</style>
