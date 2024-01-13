<template>
  <section
    class="h-[10svh] flex justify-center items-center px-2 top-0 sticky dark:bg-[#0406208d] header"
  >
    <div
      class="flex justify-between items-center w-full 2xl:max-w-[1440px] px-2"
    >
      <NuxtLink to="/"
        ><div class="flex gap-3 cursor-pointer">
          <Icon name="logos:nuxt-icon" size="1.5rem" />
          <p>TOBIAUTH</p>
        </div></NuxtLink
      >
      <div class="flex items-center gap-3">
        <div @click="isLight" class="hidden dark:flex transition">
          <Icon
            name="material-symbols:sunny"
            size="1.5rem"
            class="cursor-pointer"
            color="gray"
          />
        </div>
        <div @click="isDark" class="flex dark:hidden transition">
          <Icon
            name="material-symbols:dark-mode"
            size="1.5rem"
            class="cursor-pointer"
            color="gray"
          />
        </div>
        <a href="https://github.com/TheTobiGit/thetobiAuthDocs" target="_blank"
          ><Icon name="mdi:github" size="1.5rem " color="gray"
        /></a>
      </div>
    </div>
  </section>
</template>

<style scoped>
.header {
  backdrop-filter: blur(16px) saturate(180%);
  -webkit-backdrop-filter: blur(16px) saturate(180%);

  @apply dark:backdrop:blur-[2px];
}
</style>

<script setup>
const colorMode = useColorMode();

function isLight() {
  colorMode.value = "light";
  colorMode.preference = "light";
}

function isDark() {
  colorMode.value = "dark";
  colorMode.preference = "dark";
}
</script>
