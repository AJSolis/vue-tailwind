<script setup lang="ts">
  import { useDark, useToggle } from "@vueuse/core";

  const isDark = useDark();
  const toggleDark = useToggle(isDark);

</script>

<template>
    <nav class="bg-zinc-800	 dark:bg-neutral-50 min-h-screen shadow">
        <div class="container mx-auto px-6 py-3">
            <div class="flex justify-center items-center">
                <div class="flex space-x-6">
                    <RouterLink to="/" class="text-white dark:text-black hover:text-gray-500">Home</RouterLink>
                    <RouterLink to="/about" class="text-white dark:text-black hover:text-gray-500">About</RouterLink>
                    <RouterLink to="/contact" class="text-white dark:text-black hover:text-gray-500">Contact Me</RouterLink>
                    <RouterLink to="/tailwind" class="text-white dark:text-black hover:text-gray-500">Vue Tailwind Projects</RouterLink>
                    <RouterLink to="/resume" class="text-white dark:text-black hover:text-gray-500">Resume</RouterLink>
                    <button
                        @click="toggleDark()"
                        class=" bg-zinc-800	 text-white dark:text-black dark:bg-neutral-50 hover:text-gray-500"
                    >
                    {{ isDark ? "Dark" : "Light" }} Mode
                    </button>
                </div>
            </div>
        </div>
    </nav>
</template>