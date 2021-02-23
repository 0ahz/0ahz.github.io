<template>
  <nav class="text-xl mt-6">
    <router-link class="icon-btn mx-2" to="/">
      <icon-carbon-face-satisfied-filled />
    </router-link>
    <router-link class="icon-btn mx-2" to="/">
      <icon-carbon-campsite />
    </router-link>

    <router-link class="icon-btn mx-2" to="/">
      <span>Home</span>
    </router-link>

    <router-link class="icon-btn mx-2" to="/about">
      <span>About</span>
    </router-link>

    <router-link class="icon-btn mx-2" to="/posts">
      <span>Posts</span>
    </router-link>

    <a class="icon-btn mx-2" @click="toggleDark">
      <icon-carbon-moon v-if="isDark" />
      <icon-carbon-sun v-else />
    </a>
  </nav>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import { isDark, toggleDark } from '~/logics'

export default defineComponent({
  setup() {
    return {
      isDark,
      toggleDark,
    }
  },
})
</script>
