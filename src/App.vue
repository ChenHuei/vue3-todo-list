<template>
  <div class="layout">
    <router-view />
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'App',
  setup() {
    return {
      test: 'test',
    }
  },
})
</script>

<style lang="scss" scoped>
.layout {
  @include display-flex();

  margin-bottom: 20px;
}
</style>
