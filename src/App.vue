<template>
  <div class="layout-wrapper">
    <div class="layout-container">
      <div class="layout">
        <router-view />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'App',
  setup() {
    return {
      title: 'TODO LIST',
    }
  },
}
</script>

<style lang="scss" scoped>
.layout {
  @include size(100%, auto);
  @include display-flex();

  flex-direction: column;
  padding: 12px 16px;
}
</style>
