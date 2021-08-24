<script setup lang="ts">
// import { useRouter } from 'vue-router'
import { useI18n } from 'vue-i18n'
// import { useUserStore } from '~/stores/user'

const { t } = useI18n()
</script>

<template>
  <nav
    class="content-center fixed w-screen"
    p="y-4"
    text="2xl dark-200"
    bg="light-500"
    dark:bg="dark-200"
    dark:text="light-500"
    font="mono"
  >
    <router-link class="link-btn" m="x-4" to="/">
      <!-- icon usage: https://icones.netlify.app/ -->
      <carbon-campsite class="" />
    </router-link>

    <router-link class="link-btn" m="x-4" to="/home">
      {{ t("navbar.index") }}
    </router-link>

    <router-link class="link-btn" m="x-4" to="/skill">
      {{ t("navbar.skill") }}
    </router-link>

    <router-link class="link-btn" m="x-4" to="/experience">
      {{ t("navbar.experience") }}
    </router-link>
  </nav>
</template>
