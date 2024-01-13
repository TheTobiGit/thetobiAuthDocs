<template>
  <section class="p-4 flex justify-center min-h-[100svh]">
    <div class="2xl:max-w-[1440px] flex flex-col items-center gap-7">
      <h1 class="text-left">1. Setting up a Supabase Project:</h1>

      <div class="w-full border mb-5 border-gray-500"></div>

      <div class="textCard">
        <h2>Sign Up for a Supabase Account</h2>
        <ul class="list">
          <li>
            Visit the <a href="https://supabase.com">Supabase website </a>and
            click on the "Start for free" button.
          </li>

          <li>
            Create a Supabase account by providing your email address, password,
            and organization details.
          </li>

          <li>Once registered, log in to your Supabase account.</li>
        </ul>
      </div>

      <div class="textCard">
        <h2>Create a New Project</h2>
        <ul class="list">
          <li>
            After logging in, you'll be redirected to the dashboard. Click on
            the "Create a new project" button and select your organization.
          </li>

          <li>
            Enter a project name, set your password, select your region (I
            normally choose London), and click on the "Create Project" button.
          </li>

          <li>
            Wait for Supabase to set up your project. Once done, you'll be
            redirected to the project dashboard.
          </li>
        </ul>
      </div>

      <div class="textCard">
        <h2>Configure PostgreSQL Database</h2>
        <ul class="list">
          <li>
            In the project dashboard, locate the "Database" section and click on
            it.
          </li>
          <li>
            In the Database section, you'll find your PostgreSQL database URL.
            Make a note of this URL as it will be used to connect your Nuxt
            project to Supabase.
          </li>
        </ul>
      </div>
      <div>
        <h2>Set Up API Key</h2>
        <ul class="list">
          <li>Navigate to the "Settings" tab in the project dashboard.</li>
          <li>
            Under the "API" section, you'll find your API URL and an "API Key."
            Note down the API URL; the API Key will be used to authenticate
            requests made from your Nuxt project to Supabase.
          </li>
        </ul>
      </div>

      <div class="w-full border mb-5 border-gray-500"></div>

      <p>
        Congratulations! You've successfully set up a Supabase project. In the
        next section, we'll integrate this project with your Nuxt.js application
        using the Supabase Nuxt module.
      </p>

      <div class="flex flex-col lg:flex-row gap-6 self-end">
        <NuxtLink to="/introduction"
          ><div
            class="border rounded-md p-5 flex flex-col items-start gap-3 cursor-pointer hover:bg-gray-100 dark:hover:bg-[#2f3155d9] border-gray-500 navBox group lg:max-w-[20vw]"
          >
            <Icon
              name="material-symbols-light:arrow-circle-left-outline-rounded"
              size="2rem"
              class="icon group-hover:text-green-500 dark:text-white text-black"
            />
            <p class="text-sm dark:text-white text-black font-bold">
              Introduction
            </p>
            <p class="text-[12px] text-left dark:text-white text-black">
              Learn how to integrate Supabase into your Nuxt project
            </p>
          </div></NuxtLink
        >

        <a to="/installing-supabase-model"
          ><div
            class="border rounded-md p-5 flex flex-col items-end gap-3 cursor-pointer hover:bg-gray-100 dark:hover:bg-[#2f3155d9] border-gray-500 navBox group lg:max-w-[20vw]"
          >
            <Icon
              name="material-symbols-light:arrow-circle-right-outline-rounded"
              size="2rem"
              class="icon group-hover:text-green-500 dark:text-white text-black"
            />
            <p class="text-sm dark:text-white text-black font-bold">
              Installating the Supabase Nuxt Module
            </p>
            <p class="text-[12px] text-right dark:text-white text-black">
              Learn how to integrate Supabase into your Nuxt project
            </p>
          </div></a
        >
      </div>
    </div>
  </section>
</template>

<script setup>
useHead({
  title: "Setting up a Supabase Project",
});
</script>

<style scoped>
p,
li {
  @apply dark:text-[#d1d5db];
}
</style>
