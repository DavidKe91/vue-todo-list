<template>
  <div id="app" class="container">
    <img src="./assets/logo.png" class="logo">
    <toDoList></toDoList>
    <todolisttest></todolisttest>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld'
import toDoList from './components/todolist'
import todolisttest from './components/todolisttest'

export default {
  name: 'App',
  components: {
    HelloWorld,
    toDoList,
    todolisttest
  }
}
</script>

<style>
* {
  box-sizing: border-box;
}

.container {
  max-width: 600;
  margin: 0 auto;
}

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin-top: 60px;
  font-size: 24px;
}

.logo {
  display: block;
  height: 75px;
  margin: 20px auto;
}
</style>
