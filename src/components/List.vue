<template>
  <div class="list">
    list
    <Item v-for="item in list" :key="item.id" v-bind="item"/>
  </div>
</template>

<script>
import Item from './list/Item'

export default {
  name: 'List',
  components: { Item },
  props: {
    list: {
      type: Array,
      default() {
        return []
      }
    }
  }
}
</script>
