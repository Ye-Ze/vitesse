<script setup lang="ts">
// import { useRouter } from 'vue-router'
import { useI18n } from 'vue-i18n'
import { isDark, toggleDark } from '~/logic'
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
    font="sans"
  >
    <router-link class="link-btn" m="x-4" to="/hello">
      <!-- icon usage: https://icones.netlify.app/ -->
      <carbon-campsite class="" />
    </router-link>

    <router-link class="link-btn" m="x-4" to="/">
      {{ t("navbar.index") }}
    </router-link>

    <router-link class="link-btn" m="x-4" to="/skill">
      {{ t("navbar.skill") }}
    </router-link>

    <router-link class="link-btn" m="x-4" to="/experience">
      {{ t("navbar.experience") }}
    </router-link>
    <button class="link-btn !outline-none" :title="t('button.toggle_dark')" @click="toggleDark">
      <carbon-moon v-if="isDark" />
      <carbon-sun v-else />
    </button>
  </nav>
</template>
