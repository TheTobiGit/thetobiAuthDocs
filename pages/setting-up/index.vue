<template>
  <section class="p-4 flex justify-center min-h-[100svh]">
    <div class="2xl:max-w-[1440px] flex flex-col items-center gap-7">
      <h1 class="text-left">1. Setting up a Supabase Project:</h1>

      <div class="w-full border mb-5 border-gray-500"></div>
      <div
        class="border rounded-md p-5 flex flex-col items-end self-end gap-3 cursor-pointer hover:bg-[#2f3155d9] border-gray-500 navBox group max-w-[20vw]"
      >
        <Icon
          name="material-symbols-light:arrow-circle-right-outline-rounded"
          size="2rem"
          class="icon group-hover:text-green-500"
        />
        <p class="text-sm dark:text-white font-bold">
          Installating the Supabase Nuxt Module
        </p>
        <p class="text-[12px] text-right">
          Learn how to integrate Supabase into your Nuxt project
        </p>
      </div>
    </div>
  </section>
</template>

<script setup></script>

<style scoped>
p,
li {
  @apply dark:text-[#d1d5db];
}
</style>
