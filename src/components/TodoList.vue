<template>
  <div>
    <h3 class="list">Todo list</h3>
    <div>
      <div>
        <single-todo :todo="todo" v-for="todo in todos" :key="todo.id" />
      </div>
    </div>
  </div>
</template>

<script>
import SingleTodo from './SingleTodo'
export default {
  name: 'TodoList',
  props: ['todos'],
  components: {
    SingleTodo
  }
}
</script>
