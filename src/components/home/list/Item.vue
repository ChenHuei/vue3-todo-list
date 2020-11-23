<template>
  <div class="item">
    <h2 class="item-title">
      {{ name }}
    </h2>
    <div class="item-checked">
      {{ isCompleted ? 'check' : 'uncheck' }}
    </div>
  </div>
</template>

<script>
export default {
  name: 'Item',
  props: {
    name: {
      type: String,
      default: '',
    },
    isCompleted: {
      type: Boolean,
      default: false,
    },
  },
}
</script>

<style lang="scss" scoped>
.item {
  @include size(100%, auto);
  @include display-flex();

  padding: 8px 12px;
  &-title {
    margin-right: 12px;
  }
}
</style>
