<template>
  <div class="min-h-screen w-full bg-main">
    <layout-navbar />
    <main class="flex h-full w-full flex-col items-center py-4">
      <slot />
    </main>
    <layout-footer />
  </div>
</template>

<script lang="ts" setup></script>

<style></style>
