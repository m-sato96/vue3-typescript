<script setup lang="ts">
import { reactive } from "vue";
type User = {
  id: number;
  name: string;
};
const user1: User = reactive({
  id: 1,
  name: "鈴木",
});
user1.name = "佐藤";
</script>

<template>
  {{ user1.name }}
</template>
