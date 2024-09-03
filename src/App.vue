<script setup>
import VButton from "./components/VButton.vue";
import DataTable from "./components/DataTable.vue";
import InputDate from "./components/InputDate.vue";
import InputSearch from "./components/InputSearch.vue";
import Radio from "./components/Radio.vue";
import Textarea from "./components/Textarea.vue";
import Toggle from "./components/Toggle.vue";
import VuetifyCheckbox from "./components/VuetifyCheckbox.vue";
import InputPassword from "./components/InputPassword.vue";
import Password from "./components/Password.vue";
</script>

<template>
  <v-container>
    <VButton text="テキスト" />
    <InputPassword />
    <Password />
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
