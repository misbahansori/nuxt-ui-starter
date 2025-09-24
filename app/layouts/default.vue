<template>
  <div>
    <!-- Header with Navigation -->
    <UHeader>
      <template #left>
        <UButton
          to="/"
          color="primary"
          variant="ghost"
          size="lg"
          class="font-bold text-xl"
        >
          Nuxt UI Starter
        </UButton>
      </template>

      <template #right>
        <div class="hidden lg:flex items-center gap-6">
          <UButton to="#features" color="neutral" variant="ghost" size="sm">
            Features
          </UButton>
          <UButton
            to="https://ui.nuxt.com"
            target="_blank"
            color="neutral"
            variant="ghost"
            size="sm"
            icon="i-heroicons-book-open"
          >
            Documentation
          </UButton>
          <UButton
            to="https://github.com/nuxt/ui"
            target="_blank"
            color="neutral"
            variant="ghost"
            size="sm"
            icon="i-simple-icons-github"
          >
            GitHub
          </UButton>
          <UColorModeButton />
          <UButton
            to="https://ui.nuxt.com/pro"
            target="_blank"
            color="primary"
            variant="solid"
            size="sm"
          >
            Get Started
          </UButton>
        </div>

        <!-- Mobile menu toggle -->
        <UButton
          color="neutral"
          variant="ghost"
          size="sm"
          class="lg:hidden"
          icon="i-heroicons-bars-3"
          @click="mobileMenuOpen = !mobileMenuOpen"
        />
      </template>

      <!-- Mobile menu content -->
      <template #content>
        <div class="flex flex-col gap-4 p-4">
          <UButton
            to="#features"
            color="neutral"
            variant="ghost"
            size="lg"
            block
            @click="mobileMenuOpen = false"
          >
            Features
          </UButton>
          <UButton
            to="https://ui.nuxt.com"
            target="_blank"
            color="neutral"
            variant="ghost"
            size="lg"
            block
            icon="i-heroicons-book-open"
            @click="mobileMenuOpen = false"
          >
            Documentation
          </UButton>
          <UButton
            to="https://github.com/nuxt/ui"
            target="_blank"
            color="neutral"
            variant="ghost"
            size="lg"
            block
            icon="i-simple-icons-github"
            @click="mobileMenuOpen = false"
          >
            GitHub
          </UButton>
          <div class="flex items-center justify-between">
            <span class="text-sm font-medium">Theme</span>
            <UColorModeButton />
          </div>
          <UButton
            to="https://ui.nuxt.com/pro"
            target="_blank"
            color="primary"
            variant="solid"
            size="lg"
            block
            @click="mobileMenuOpen = false"
          >
            Get Started
          </UButton>
        </div>
      </template>
    </UHeader>

    <!-- Main content -->
    <slot />
  </div>
</template>

<script setup>
const mobileMenuOpen = ref(false);
</script>
