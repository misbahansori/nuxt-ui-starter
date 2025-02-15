<script setup lang="ts">
const colorMode = useColorMode();
</script>

<template>
  <section>
    <div class="max-w-5xl mx-auto px-4 py-20">
      <Button icon="heroicons:user" loading variant="subtle"> Button </Button>

      <Select v-model="colorMode.preference" :options="['light', 'dark']" />
    </div>
  </section>
</template>
