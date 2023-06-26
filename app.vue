<template>
  <div
    class="flex flex-col min-h-screen overflow-hidden font-inter antialiased text-heading tracking-tight bg-surface"
    :class="isDarkTheme ? 'theme-dark' : 'theme-light'"
  >
    <Header />
    <NuxtPage />
    <Footer />
  </div>
</template>
<script setup>
import useTheme from "@/composables/useTheme";
const { isDarkTheme } = useTheme();

useHead({
  script: [
    {
      src: "https://scripts.simpleanalyticscdn.com/latest.js",
      async: true,
    },
  ],
});
</script>