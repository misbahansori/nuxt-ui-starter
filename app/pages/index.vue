<template>
  <div>
    <UPageHero
      title="Build Amazing Web Applications"
      description="Create stunning, responsive web applications with Nuxt UI. Get started with our comprehensive component library and modern development tools."
      :links="[
        {
          label: 'Get Started',
          to: '#features',
          color: 'primary',
          variant: 'solid',
        },
        {
          label: 'View Documentation',
          to: 'https://ui.nuxt.com',
          color: 'neutral',
          variant: 'outline',
        },
      ]"
    >
      <template #headline>
        <UBadge
          color="primary"
          variant="subtle"
          size="lg"
          class="relative rounded-full font-semibold"
        >
          <span
            class="absolute inset-0 w-full h-full bg-primary-500/20 rounded-full animate-pulse"
          />
          <span class="relative">New in v4.0</span>
        </UBadge>
      </template>
    </UPageHero>
  </div>
</template>
