<script lang="ts">
// give each todo a unique id
let id = 0

export default {
  data() {
    return {
      newTodo: '',
      hideCompleted: false,
      todos: [
        { id: id++, text: 'Learn HTML', done: true },
        { id: id++, text: 'Learn JavaScript', done: true },
        { id: id++, text: 'Learn Vue', done: false }
      ]
    }
  },
  computed: {
    filteredTodos() {
      return this.hideCompleted
        ? this.todos.filter((t) => !t.done)
        : this.todos
    }
  },
  methods: {
    addTodo() {
      if (this.newTodo === "") {
        alert("SORRY BUT THIS TODO CANNOT BE EMPTY")
        return;
      }
      this.todos.push({ id: id++, text: this.newTodo, done: false })
      // ...
      this.newTodo = ''
    },
    removeTodo(todo: any) {

      this.todos = this.todos.filter(item => item.id !== todo.id)
      // ...
    }
  }
}
</script>

<template>



  <div class="classBox">

    <h1>##07 TODO LIST</h1>

    <form @submit.prevent="addTodo">
      <div class="box-button">
        <input v-model="newTodo">

        <button class="button-85">Add Todo</button>
      </div>
    </form>
    <ul>
      <li class="list" v-for="todo in filteredTodos" :key="todo.id">
        <input type="checkbox" v-model="todo.done" />
        <span :class="{ done: todo.done }">{{ todo.text }}</span>
        <button class="button-24" @click="removeTodo(todo)">X</button>
      </li>
    </ul>
    <div class="box-button">
      <button class="button-24" @click="hideCompleted = !hideCompleted">
        {{ hideCompleted ? 'Show all' : 'Hide completed' }}
      </button>
    </div>
  </div>
</template>

<style scoped>
.done {
  text-decoration: line-through;
}
</style>