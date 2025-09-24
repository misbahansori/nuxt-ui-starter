<template>
  <div>
    <!-- Hero Section -->
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

    <!-- Features Section -->
    <UPageSection>
      <UPageHeader
        title="Why Choose Nuxt UI?"
        description="Discover the features that make Nuxt UI the perfect choice for your next project"
        align="center"
      />

      <UPageGrid>
        <UPageFeature
          title="Lightning Fast"
          description="Built with performance in mind. Nuxt UI components are optimized for speed and efficiency."
          icon="i-heroicons-bolt"
        />
        <UPageFeature
          title="Beautiful Design"
          description="Carefully crafted components with modern design principles and accessibility in mind."
          icon="i-heroicons-paint-brush"
        />
        <UPageFeature
          title="Responsive"
          description="All components are fully responsive and work seamlessly across all device sizes."
          icon="i-heroicons-device-phone-mobile"
        />
        <UPageFeature
          title="Easy to Use"
          description="Simple API with TypeScript support. Get started in minutes with our comprehensive documentation."
          icon="i-heroicons-wrench-screwdriver"
        />
        <UPageFeature
          title="Dark Mode"
          description="Built-in dark mode support with automatic theme switching and customization options."
          icon="i-heroicons-moon"
        />
        <UPageFeature
          title="Accessible"
          description="WCAG compliant components with proper ARIA attributes and keyboard navigation support."
          icon="i-heroicons-heart"
        />
      </UPageGrid>
    </UPageSection>

    <!-- Stats Section -->
    <UPageSection
      class="bg-gradient-to-br from-primary-50 to-primary-100 dark:from-gray-900 dark:to-gray-800 relative overflow-hidden"
    >
      <!-- Background decoration -->
      <div class="absolute inset-0 bg-grid-pattern opacity-5"></div>
      <div
        class="absolute top-0 left-1/4 w-72 h-72 bg-primary-200/20 rounded-full blur-3xl"
      ></div>
      <div
        class="absolute bottom-0 right-1/4 w-96 h-96 bg-primary-300/20 rounded-full blur-3xl"
      ></div>

      <UContainer class="relative">
        <div class="text-center mb-12">
          <h2 class="text-3xl font-bold text-gray-900 dark:text-white mb-4">
            Trusted by Developers Worldwide
          </h2>
          <p class="text-lg text-gray-600 dark:text-gray-300 max-w-2xl mx-auto">
            Join thousands of developers who are building amazing applications
            with Nuxt UI
          </p>
        </div>

        <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
          <!-- Stat 1 -->
          <div>
            <div
              class="bg-white/80 dark:bg-gray-800/80 backdrop-blur-sm rounded-2xl p-8 shadow-lg border border-white/20"
            >
              <div
                class="flex items-center justify-center w-12 h-12 bg-primary-100 dark:bg-primary-900/30 rounded-full mx-auto mb-4"
              >
                <UIcon
                  name="i-heroicons-cube"
                  class="w-6 h-6 text-primary-600 dark:text-primary-400"
                />
              </div>
              <div
                class="text-5xl font-bold text-primary-600 dark:text-primary-400 mb-2"
              >
                100+
              </div>
              <div class="text-gray-600 dark:text-gray-300 font-medium">
                Components
              </div>
              <div class="text-sm text-gray-500 dark:text-gray-400 mt-1">
                Ready to use
              </div>
            </div>
          </div>

          <!-- Stat 2 -->
          <div>
            <div
              class="bg-white/80 dark:bg-gray-800/80 backdrop-blur-sm rounded-2xl p-8 shadow-lg border border-white/20"
            >
              <div
                class="flex items-center justify-center w-12 h-12 bg-green-100 dark:bg-green-900/30 rounded-full mx-auto mb-4"
              >
                <UIcon
                  name="i-heroicons-arrow-down-tray"
                  class="w-6 h-6 text-green-600 dark:text-green-400"
                />
              </div>
              <div
                class="text-5xl font-bold text-green-600 dark:text-green-400 mb-2"
              >
                50k+
              </div>
              <div class="text-gray-600 dark:text-gray-300 font-medium">
                Downloads
              </div>
              <div class="text-sm text-gray-500 dark:text-gray-400 mt-1">
                Monthly active
              </div>
            </div>
          </div>

          <!-- Stat 3 -->
          <div>
            <div
              class="bg-white/80 dark:bg-gray-800/80 backdrop-blur-sm rounded-2xl p-8 shadow-lg border border-white/20"
            >
              <div
                class="flex items-center justify-center w-12 h-12 bg-purple-100 dark:bg-purple-900/30 rounded-full mx-auto mb-4"
              >
                <UIcon
                  name="i-heroicons-heart"
                  class="w-6 h-6 text-purple-600 dark:text-purple-400"
                />
              </div>
              <div
                class="text-5xl font-bold text-purple-600 dark:text-purple-400 mb-2"
              >
                99%
              </div>
              <div class="text-gray-600 dark:text-gray-300 font-medium">
                Satisfaction
              </div>
              <div class="text-sm text-gray-500 dark:text-gray-400 mt-1">
                Developer rating
              </div>
            </div>
          </div>
        </div>

        <!-- Additional stats row -->
        <div class="grid grid-cols-2 md:grid-cols-4 gap-6 mt-12">
          <div class="text-center">
            <div class="text-2xl font-bold text-gray-700 dark:text-gray-300">
              24/7
            </div>
            <div class="text-sm text-gray-500 dark:text-gray-400">Support</div>
          </div>
          <div class="text-center">
            <div class="text-2xl font-bold text-gray-700 dark:text-gray-300">
              MIT
            </div>
            <div class="text-sm text-gray-500 dark:text-gray-400">License</div>
          </div>
          <div class="text-center">
            <div class="text-2xl font-bold text-gray-700 dark:text-gray-300">
              100%
            </div>
            <div class="text-sm text-gray-500 dark:text-gray-400">
              Open Source
            </div>
          </div>
          <div class="text-center">
            <div class="text-2xl font-bold text-gray-700 dark:text-gray-300">
              v4.0
            </div>
            <div class="text-sm text-gray-500 dark:text-gray-400">Latest</div>
          </div>
        </div>
      </UContainer>
    </UPageSection>

    <!-- CTA Section -->
    <UPageCTA
      title="Ready to Get Started?"
      description="Join thousands of developers building amazing applications with Nuxt UI"
      :links="[
        {
          label: 'Start Building',
          to: 'https://ui.nuxt.com',
          color: 'primary',
          variant: 'solid',
        },
        {
          label: 'View Examples',
          to: 'https://ui.nuxt.com/pro',
          color: 'neutral',
          variant: 'outline',
        },
      ]"
    />

    <!-- Footer -->
    <UFooter>
      <template #left>
        <p class="text-gray-500 dark:text-gray-400 text-sm">
          © 2024 Nuxt UI Starter. Built with ❤️ using Nuxt UI.
        </p>
      </template>

      <template #right>
        <div class="flex gap-4">
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
        </div>
      </template>
    </UFooter>
  </div>
</template>
