<template>
    <v-container>
      <!-- トグルスイッチ -->
      <v-switch
        v-model="isOn"
        label="Enable feature"
      ></v-switch>
  
      <!-- トグルスイッチの状態を表示 -->
      <v-alert v-if="isOn" type="info">
        Feature is enabled
      </v-alert>
      <v-alert v-else type="warning">
        Feature is disabled
      </v-alert>
    </v-container>
  </template>
  
  <script setup>
  import { ref } from 'vue';
  
  const isOn = ref(false);
  </script>
  