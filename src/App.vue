<template>
  <v-app>
    <v-main>
      <v-app-bar elevation="1">
        <nav>
          <router-link to="/">
            {{ $t('navigation.home') }}
          </router-link>
          |
          <router-link to="/about">{{ $t('navigation.about') }}</router-link>
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
<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #7bc6ff;
    }
  }
}
</style>
