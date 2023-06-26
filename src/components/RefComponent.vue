<script setup lang="ts">
import { ref, type Ref } from "vue";

// const count = ref<number>(0);
const count: Ref<number> = ref(0);
</script>

<template>
  <h1>RefComponent</h1>
  {{ count }}
  <button @click="count++">クリック</button>
</template>
