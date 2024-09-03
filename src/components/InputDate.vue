<script setup>
import { ref, computed } from "vue";

const date = ref("");
const rules = {
  required: (value) => !!value || "Date is required",
};
</script>

<template>
  <v-container>
    <!-- 日付入力フィールド -->
    <v-text-field
      v-model="date"
      type="date"
      :rules="[rules.required]"
      hint="Select a date in YYYY-MM-DD format"
      append-icon="mdi-calendar"
    ></v-text-field>
  </v-container>
</template>
