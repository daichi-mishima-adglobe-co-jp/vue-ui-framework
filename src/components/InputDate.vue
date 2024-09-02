<template>
  <v-container>
    <!-- 日付入力フィールド -->
    <v-text-field
      v-model="date"
      label="Select a date"
      type="date"
      :rules="[rules.required]"
      hint="Select a date in YYYY-MM-DD format"
      append-icon="mdi-calendar"
    ></v-text-field>

    <!-- 選択された日付の表示 -->
    <v-alert v-if="date" type="info">
      Selected Date: {{ formattedDate }}
    </v-alert>
  </v-container>
</template>

<script setup>
import { ref, computed } from "vue";

const date = ref("");
const rules = {
  required: (value) => !!value || "Date is required",
};

const formattedDate = computed(() => {
  if (date.value) {
    return new Date(date.value).toLocaleDateString();
  }
  return "";
});
</script>

<style scoped>
/* カレンダーアイコンを右に寄せるスタイルをカスタマイズ */
.v-input__append-inner {
  margin-left: auto;
}
</style>
