<script setup lang="ts">
const handleChange = (e: Event) => {
  console.log((e.target as HTMLInputElement).value);
};
const handleClick = () => {
  console.log("クリックされました");
};
</script>

<template>
  <input type="text" @change="handleChange" />
  <button @click="handleClick">クリック</button>
</template>
