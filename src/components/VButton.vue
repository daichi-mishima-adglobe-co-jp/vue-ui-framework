<script setup>
defineProps(["text"]);
</script>

<template>
  <v-btn class="bg-black max-w-[320px] w-full h-12" variant="flat"
    >{{ text }}
  </v-btn>
</template>
