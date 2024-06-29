<template>
  <div class="flex min-h-screen w-full flex-col bg-main">
    <layout-navbar />
    <main class="flex h-full w-full flex-col items-center py-4">
      <slot />
    </main>
    <layout-footer />
  </div>
</template>
