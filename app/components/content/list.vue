<template>
  <div
    class="my-2 flex w-full flex-col"
    :class="side === 'right' ? 'items-end' : 'items-start'"
  >
    <b class="text-2xl"><ContentSlot :use="$slots.default" unwrap="p" /></b>
    <ul
      class="flex flex-col"
      :class="side === 'right' ? 'items-end' : 'items-start'"
    >
      <li v-for="item in items" :key="item">{{ item }}</li>
    </ul>
  </div>
</template>
<script lang="ts" setup>
defineProps<{
  items: string[];
  side?: "left" | "right";
}>();
</script>
