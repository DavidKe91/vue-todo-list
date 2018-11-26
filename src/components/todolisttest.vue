<template>
  <div>
    <input class="todo-input" type="text" placeholder="What needs to be done" v-model="newtodo" @keyup.enter="addToArray">
    <div class="todo-item" v-for="todo in todos" :key="todo.id">{{todo.title}}</div>
  </div>
</template>

<script>
  export default {
    name: 'todolisttest',
    data () {
      return {
        newtodo: '',
        idfortodotest: 3,
        todos: [
          {
            'id': 1,
            'title': 'First Title',
            'completed': false,
          },
          {
            'id': 2,
            'title': 'Second Title',
            'completed': false,
          },
        ]
      }
    },
    methods: {
      addToArray(){
      this.todos.push({
        id: this.idfortodotest,
        title: this.newtodo,
        completed: false,
      })
      this.idfortodotest++
      this.newtodo = ''
      }
      }
  }
</script>
