<script setup lang="ts">
defineProps<{ color: string }>()

const sendAlert = () => alert('Hello :)')
</script>

<template>
  <button @click="sendAlert" :style="{ color }">
    <slot />
  </button>
</template>
