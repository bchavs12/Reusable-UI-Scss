<script setup lang="ts">
import { PhPlusCircle } from "@phosphor-icons/vue"
</script>

<template>
  <form>
    <input
      type="text"
      placeholder="Add a New Task"
      required
      class="input-task"
    />
    <button type="submit" class="btn-add-task" disabled>
      ADD
      <PhPlusCircle size="16" color="#f2f2f2" weight="bold" />
    </button>
  </form>
</template>

<style scoped lang="scss">
@import "../scss/variables";

form {
  display: flex;
  flex: 1 1 0%;
  gap: 0.5rem;
  justify-content: space-between;
  .input-task {
    width: 100%;
    border: 1px solid $gray-700;
    border-radius: $rounded-lg;
    background: $bg-base-gray-500;
    color: $text-gray-100;
    padding: 1rem;
    &::placeholder {
      color: $text-gray-300;
    }
    &:focus {
      border-color: $purple-dark;
    }
  }
  .btn-add-task {
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 0.5rem; //8px
    background: $blue-dark;
    color: $text-gray-100;
    border-radius: $rounded-lg;
    padding: 1rem;
    cursor: pointer;
  }
}
</style>
