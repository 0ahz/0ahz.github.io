<template>
  <footer>
    <span>Made in Beijing</span>
    <span> • </span>
    <span>Mark Zhao</span>
    <span> • </span>
    <span>{{ year }}</span>
    <a
      class="mx-2"
      rel="noreferrer"
      href="https://github.com/0ahz/0ahz.github.io"
      target="_blank"
      title="GitHub"
    >
      <icon-carbon-logo-github />
    </a>
  </footer>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  setup() {
    return {
      year: new Date().getFullYear(),
    }
  },
})
</script>
