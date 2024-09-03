<script setup>
    import {ref
    } from "vue"

    const text = ref("")

    const showPassword = ref(false)

    const handleToggle = () => {
        showPassword.value = !showPassword.value
    }
</script>

<template>
    <div class="relative">
        <input v-model="text" :type="showPassword ? 'text' : 'password'" class="border border-gray-200 rounded text-md pl-2 py-2 pr-10 w-full focus-visible:outline-black" placeholder="パスワードを入力してください" />
        <button class="absolute top-1/2 right-2 -translate-y-1/2" @click="handleToggle">
            <v-icon>{{ showPassword ? 'mdi-eye-off' : 'mdi-eye' }}</v-icon>
        </button>
    </div>
</template>