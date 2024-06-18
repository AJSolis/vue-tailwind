<script setup lang="ts">
  import { useDark, useToggle } from "@vueuse/core";

  const isDark = useDark();
  const toggleDark = useToggle(isDark);

  import headerfile from '../components/header.vue'
</script>

<template>
  <headerfile />
  
</template>
