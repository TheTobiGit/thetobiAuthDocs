<template>
  <section class="p-4 flex justify-center min-h-[100svh]">
    <div class="2xl:max-w-[1440px] flex flex-col items-center gap-7">
      <h1 class="text-left">2. Installing the Supabase Module:</h1>

      <div class="w-full border mb-5 border-gray-500"></div>

      <p class="text left text-balance self-start">
        Now that you have a Supabase project set up, it's time to integrate it
        into your Nuxt.js application using the official Supabase Nuxt module.
      </p>

      <div class="textCard">
        <h2>Create a Nuxt.js Project</h2>
        <div class="textCard mb-4">
          <p class="font-bold">Prerequisites</p>
          <ul class="list before:text-[#f8fafc]">
            <li>
              <b>Node.js </b>-
              <span
                class="p-1 border border-dashed dark:bg-[#1d293b] bg-[#f8fafc] rounded-sm text-bold border-gray-400"
                >v18.0.0</span
              >
              or newer
            </li>
            <li>
              <b>Text editor </b>- Official Nuxt Documentation recommenda
              <a href="https://code.visualstudio.com/">Visual Studio Code</a>
              with the
              <a
                href="https://marketplace.visualstudio.com/items?itemName=Vue.volar"
                >Volar Extension</a
              >
            </li>
            <li><b>Terminal</b> - In order to run Nuxt commands</li>
          </ul>
        </div>

        <p>
          If you don't have a Nuxt.js project yet, create one using the
          following command in your terminal:
        </p>
        <pre class="bg-[#f8fafc] text-green-500">
  <code>
    npx nuxi@latest init project-name
  </code>
</pre>
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
            class="border rounded-md p-5 flex flex-col items-start gap-3 cursor-pointer hover:bg-[#2f3155d9] border-gray-500 navBox group lg:max-w-[20vw]"
          >
            <Icon
              name="material-symbols-light:arrow-circle-left-outline-rounded"
              size="2rem"
              class="icon group-hover:text-green-500"
            />
            <p class="text-sm dark:text-white font-bold">Introduction</p>
            <p class="text-[12px] text-left">
              Learn how to integrate Supabase into your Nuxt project
            </p>
          </div></NuxtLink
        >

        <div
          class="border rounded-md p-5 flex flex-col items-end gap-3 cursor-pointer hover:bg-[#2f3155d9] border-gray-500 navBox group lg:max-w-[20vw]"
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
    </div>
  </section>
</template>

<script setup>
useHead({
  title: "Installing the Supabase Module",
});
</script>

<style scoped>
p,
li {
  @apply dark:text-[#d1d5db];
}
</style>
