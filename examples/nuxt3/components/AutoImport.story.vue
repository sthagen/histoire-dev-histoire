<script setup>
console.log('useNuxtApp', useNuxtApp())
console.log('useNuxtApp().$config', useNuxtApp().$config)
const config = useRuntimeConfig()
console.log('useRuntimeConfig', config)
</script>

<template>
  <Story>
    <Meow />

    <h3>Nuxt runtime config</h3>
    <pre>{{ config }}</pre>
    <p data-testid="config">
      {{ config.public.configFromNuxt }}
    </p>
  </Story>
</template>
