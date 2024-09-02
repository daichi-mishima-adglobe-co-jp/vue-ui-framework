<script setup>
import DataTable from "./components/DataTable.vue";
import InputDate from "./components/InputDate.vue";
import InputSearch from "./components/InputSearch.vue";
import Radio from "./components/Radio.vue";
import Textarea from "./components/Textarea.vue";
import Toggle from "./components/Toggle.vue";
import VuetifyCheckbox from "./components/VuetifyCheckbox.vue";
</script>

<template>
  <v-container>
    <v-btn>Enabled Button</v-btn>
    <v-text-field type="password"></v-text-field>
    <InputDate />
    <InputSearch />
    <Textarea />
    <VuetifyCheckbox />
    <Radio />
    <Toggle />
    <DataTable />
  </v-container>
</template>
