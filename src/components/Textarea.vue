<template>
  <v-textarea
    v-model="text"
    label="コメント"
    placeholder="ここにコメントを入力してください"
    rows="4"
    auto-grow
  ></v-textarea>
</template>

<script setup>
import { ref } from "vue";

const text = ref("");
</script>
