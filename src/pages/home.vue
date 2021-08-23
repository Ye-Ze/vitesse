<script setup lang="ts">
import { useI18n } from 'vue-i18n'
const { t } = useI18n()
</script>

<template>
  <div class="container mx-auto">
    <p class="text">
      hello world.
    </p>
  </div>
</template>

<route lang="yaml">
meta:
  layout: home
</route>
