<template>
  <router-view />
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import { useHead } from '@vueuse/head'

export default defineComponent({
  setup() {
    // https://github.com/vueuse/head
    // you can use this to manipulate the document head in any components,
    // they will be renedered correctly in the html results with vite-ssg
    useHead({
      title: '0ahz',
      meta: [
        { name: 'keywords', content: '0ahz' },
        { name: 'description', content: '0ahz' },
      ],
    })
    return {}
  },
})
</script>
