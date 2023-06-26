<script setup lang="ts">
const emit = defineEmits<{
  (e: "emitClick", message: string): void;
}>();

const childFn = (message: string): void => {
  emit("emitClick", message);
};
</script>

<template>
  <button @click="childFn('子コンポーネントでクリックされました')">クリック</button>
</template>
