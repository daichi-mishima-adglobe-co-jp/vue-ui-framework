<!-- src/components/PasswordField.vue -->
<template>
    <v-text-field
      :type="showPassword ? 'text' : 'password'"
      v-model="password"
      :append-icon="showPassword ? 'mdi-eye-off' : 'mdi-eye'"
      @click:append="togglePasswordVisibility"
      outlined
    />
  </template>
  
  <script setup>
  import { ref } from 'vue';
  
  const password = ref('');
  const showPassword = ref(false);
  
  const togglePasswordVisibility = () => {
    showPassword.value = !showPassword.value;
  };
  </script>
  
  <style scoped>
  </style>