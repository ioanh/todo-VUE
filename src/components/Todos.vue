<template>
  <div>
    <div v-bind:key="todo" v-for="todo in todos">
      <TodoItem v-bind:todo="todo" />
    </div>
  </div>
</template>>
<script>
import TodoItem from './TodoItem.vue'
export default {
  name: "Todos",
  components: {
      TodoItem
  },
  props: ["todos"]
}
</script>>
<style lang="stylus" scoped>

</style>