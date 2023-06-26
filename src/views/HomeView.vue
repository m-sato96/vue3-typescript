<script setup lang="ts">
import RefComponent from "@/components/RefComponent.vue";
import ReactiveComponent from "@/components/ReactiveComponent.vue";
import EventComponent from "@/components/EventComponent.vue";
import ComputedComponent from "@/components/ComputedComponent.vue";
import defineEvent from "@/components/DefinePropsComponent.vue";

// const items = [
//   {
//     id: 1,
//     name: "商品1",
//   },
//   {
//     id: 2,
//     name: "商品2",
//   },
//   {
//     id: 3,
//     name: "商品3",
//   },
// ];

const parentFn = (message: string): void => {
  console.log(message);
};
</script>

<template>
  <main>
    <!-- <RefComponent /> -->
    <!-- <ReactiveComponent /> -->
    <!-- <EventComponent /> -->
    <!-- <ComputedComponent /> -->
    <defineEvent @emit-click="parentFn" />
  </main>
</template>
