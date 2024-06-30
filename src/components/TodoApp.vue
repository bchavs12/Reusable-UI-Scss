<script setup lang="ts">
import TodoForm from "./TodoForm.vue"
import TodoInfo from "./TodoInfo.vue"
import TodoItem from "./TodoItem.vue"
import TodoEmpty from "./TodoEmpty.vue"
</script>

<template>
  <TodoForm />
  <section>
    <TodoInfo />
    <div>
      <TodoItem />
      <TodoEmpty />
    </div>
  </section>
</template>

<style scoped lang="scss">
section {
  margin-top: 4rem;
}
</style>
