<template>
  <h1 class="home-title">
    {{ title }}
  </h1>
  <List :list="list" />
</template>

<script>
import List from '@/components/home/List'

const LIST = [
  {
    id: 0,
    name: 'test1',
    isCompleted: true,
  },
  {
    id: 1,
    name: 'test2',
    isCompleted: false,
  },
]

export default {
  components: { List },
  setup() {
    return {
      list: LIST,
      title: 'TODO LIST',
    }
  },
}
</script>
