<template>
  <section class="p-4 flex justify-center min-h-[100svh]">
    <div class="2xl:max-w-[1440px] flex flex-col items-center gap-7">
      <h1 class="text-left">Getting Started with Supabase in Nuxt Projects</h1>
      <p class="text-balance text-left">
        Welcome to the world of Supabase and Nuxt.js! In this documentation,
        I'll guide you through the process of integrating
        <a href="https://supabase.com" target="_blank" class="">Supabase</a>, an
        open-source Firebase alternative, into your Nuxt.js projects. Supabase
        provides a set of tools and services that developers can use to quickly
        set up and manage databases, authentication, and other backend
        functionalities.
      </p>

      <div class="w-full border border-gray-500"></div>

      <div class="flex flex-col gap-2">
        <h2>Why Nuxt.js?</h2>
        <p class="text-balance">
          Nuxt.js is a powerful framework for building Vue.js applications. It
          abstracts away much of the complex setup and configuration, enabling
          developers to focus on building robust and efficient web applications.
          With its modular architecture and conventions, Nuxt.js is an excellent
          choice for creating modern, server-side rendered (SSR) applications.
          And also, that is the framework is the framework I use so... if you
          are not a nuxt developer, sorry?
        </p>
      </div>

      <div class="flex-col flex gap-3 mb-5">
        <h2>Combining Supabase and Nuxt.js</h2>
        <p class="text-balance">
          By integrating Supabase into your Nuxt projects, you can create
          feature-rich applications with a scalable backend infrastructure. This
          combination allows you to handle data storage, authentication, and
          real-time updates seamlessly, providing a solid foundation for your
          web applications.
        </p>

        <p>
          In this documentation, I'll walk you through the step-by-step process
          of setting up Supabase in a Nuxt project, covering topics such as:
        </p>

        <ul class="flex flex-col gap-1">
          <li>
            <NuxtLink to="./setting-up"
              >1. Setting up a Supabase Project:</NuxtLink
            >
            Create a Supabase project and configure it to suit the needs of your
            Nuxt application.
          </li>

          <li>
            <a>2. Installing the Supabase Nuxt Module:</a> Learn how to
            integrate Supabase into your Nuxt project using the official
            Supabase Nuxt module.
          </li>

          <li>
            <a>3. Authentication:</a> Implement user authentication using
            Supabase to secure your application and control access to resources.
          </li>

          <li>
            <a>4. Database Operations:</a> Perform CRUD (Create, Read, Update,
            Delete) operations on your PostgreSQL database using Supabase's
            intuitive API.
          </li>

          <li>
            <a>5. Real-time Updates:</a> Leverage Supabase's real-time features
            to enable instant updates in your Nuxt application.
          </li>
        </ul>
      </div>
      <div class="w-full border mb-5 border-gray-500"></div>
      <NuxtLink to="/setting-up"
        ><div
          class="border rounded-md p-5 flex flex-col items-end self-end gap-3 cursor-pointer hover:bg-gray-100 dark:hover:bg-[#2f3155d9] border-gray-500 navBox group lg:max-w-[20vw]"
        >
          <Icon
            name="material-symbols-light:arrow-circle-right-outline-rounded"
            size="2rem"
            class="icon group-hover:text-green-500"
          />
          <p class="text-sm dark:text-white font-bold">
            Setting up a Supabase Project
          </p>
          <p class="text-[12px] text-right">
            Create a Supabase project and configure it to suit the needs of your
            Nuxt application.
          </p>
        </div></NuxtLink
      >
    </div>
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
