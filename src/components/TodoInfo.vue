<script setup lang="ts"></script>

<template>
  <header class="header-todo-info">
    <aside>
      <p class="created-task-label">Created Tasks:</p>
      <span class="counter-tasks"> 5 </span>
    </aside>

    <aside>
      <p class="completed-task-label">Completed</p>
      <span class="counter-tasks"> 5 of 5</span>
    </aside>
  </header>
</template>

<style scoped lang="scss">
@import "../scss/variables";

.header-todo-info {
  display: flex;
  justify-content: space-between;
  margin-bottom: 1.5rem; //24px

  aside {
    display: flex;
    gap: 0.5rem;
    align-items: center;
    justify-content: center;
    & > .created-task-label {
      @include task-label;
    }
    & > .completed-task-label {
      @include task-label(color, $purple);
    }
  }
}
</style>
