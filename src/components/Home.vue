<template>
  <div>
    <h1 class="teal white-text">Home</h1>
    <div class="container">
      <Form />
      <todo-list :todos="todos" />
    </div>
  </div>
</template>

<script>
import Form from './Form'
import TodoList from './TodoList'
export default {
  name: 'Home',
  components: {
    Form,
    TodoList
  },
  data () {
    return {
      todos: [
        {
          id: 1,
          title: 'Title 1',
          status: false
        },
        {
          id: 2,
          title: 'Title 2',
          status: true
        },
        {
          id: 3,
          title: 'Title 3',
          status: false
        }
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1,
h2 {
  font-weight: normal;
  margin: 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
