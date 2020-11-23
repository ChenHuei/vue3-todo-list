<template>
  <h2>TODO LIST</h2>
  <List />
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import List from '@/components/List.vue'

export default defineComponent({
  components: { List },
  name: 'App',
  setup () {
    return {
    }
  }
})
</script>
