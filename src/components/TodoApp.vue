<script setup lang="ts">
import TodoForm from "./TodoForm.vue"
import TodoInfo from "./TodoInfo.vue"
import TodoItem from "./TodoItem.vue"
import TodoEmpty from "./TodoEmpty.vue"
</script>

<template>
  <TodoForm />
  <section class="mt-16">
    <TodoInfo />
    <div>
      <TodoItem />
      <TodoEmpty />
    </div>
  </section>
</template>
