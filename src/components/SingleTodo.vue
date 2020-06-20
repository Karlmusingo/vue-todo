<template>
  <div class="single-todo inline">
    <!-- <i class="material-icons right">check</i> -->
    <label>
      <input type="checkbox" :checked="todo.status" />
      <span>{{todo.title}}</span>
    </label>
  </div>
</template>

<script>
export default {
  name: 'SingleTodo',
  props: ['todo']
}
</script>
