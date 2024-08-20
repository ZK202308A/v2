<template>
  <div>
    <TodoInput @addTodo="addTodo"></TodoInput>
    <TodoList></TodoList>
  </div>
</template>

<script setup>
import { ref } from 'vue';
import TodoInput from './TodoInput.vue';
import TodoList from './TodoList.vue';
import { v4 as uuidv4 } from 'uuid';

const todoList = ref([])

const addTodo = (todo) => {
  todo.tno = uuidv4()
  todoList.value = [...todoList.value, todo]
  
  console.log(todoList.value)
}



</script>

<style  scoped>



</style>