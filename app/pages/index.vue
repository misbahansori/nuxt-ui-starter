<script setup lang="ts">
const colorMode = useColorMode();
</script>

<template>
  <section>
    <div class="max-w-5xl mx-auto px-4 py-20">
      <Button
        @click="
          colorMode.preference =
            colorMode.preference === 'dark' ? 'light' : 'dark'
        "
        >Toggle Theme</Button
      >
    </div>
  </section>
</template>
