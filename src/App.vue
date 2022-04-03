<template>
  <v-app>
    <v-main>
      <v-app-bar elevation="1">
        <nav>
          <router-link to="/">
            {{ $t('navigation.home') }}
          </router-link>
          |
          <router-link to="/about">
            {{ $t('navigation.about') }}
          </router-link>
        </nav>
      </v-app-bar>
      <router-view />
    </v-main>
  </v-app>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
export default defineComponent({
  name: 'App',

  data() {
    return {}
  }
})
</script>
<style lang="sass" scoped>
@import '@/styles/index.scss'
</style>
