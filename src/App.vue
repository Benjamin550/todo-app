<template>
  <main>
      <div class="container">
          <h1>Benjamin's Todo_App</h1>
         <todo-add></todo-add>
          <todo-filter></todo-filter>
          <todo-list></todo-list>

      </div>
  </main>
</template>

<script>
import TodoAdd from './components/TodoAdd.vue'
import TodoFilter from './components/TodoFilter'
import TodoList from './components/TodoList'
export default {
  name: 'App',
  components: {
    TodoAdd,
    TodoList,
      TodoFilter
  }
}
</script>

<style>
    *{
        box-sizing: border-box;
        margin: 0;
        padding: 0;
    }
main {
  width: 100vw;
  min-height: 100vh;
  padding: 10vh 0;
  display: grid;
  align-items: start;
  justify-items: center;
  background: #d8dfff;
}
.container {
  width: 60%;
  max-width: 400px;
  box-shadow: 0px 0px 24px rgba(0, 0, 0, 0.15);
  border-radius: 24px;
  padding: 48px 28px;
  background-color: rgb(245, 246, 252);
}
/* 标题 */
h1 {
  margin: 24px 0;
  font-size: 28px;
  color: #414873;
}
/* 添加框 */




</style>
