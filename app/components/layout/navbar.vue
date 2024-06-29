<template>
  <header class="flex w-full justify-between bg-accent p-2">
    <span class="font-mono text-xl">hozza.dev</span>
    <nav class="flex items-center gap-x-4">
      <nuxt-link v-for="link in LINKS" :to="link.path" :key="link.path">
        {{ link.name }}
      </nuxt-link>
    </nav>
  </header>
</template>

<script lang="ts" setup>
const LINKS = [
  { name: "Home", path: "/" },
  { name: "Blog", path: "/blog" },
  { name: "Projects", path: "/projects" },
  { name: "Contact", path: "/contact" },
];
</script>
