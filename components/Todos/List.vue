<template>
  <div class="max-w-md mx-auto bg-gray-200 p-10">
    <div class="text-center font-bold uppercase">Your Todo Items</div>

    <TodosTodoItem
      @showButtonClicked="showTodo"
      v-for="todo in todos"
      :key="todo.id"
      :title="todo.title"
      :desc="todo.desc"
    />
  </div>
</template>


<script>
export default {
  props: {
    todos: Array,
  },

  methods: {
    showTodo(my_data) {
      alert(my_data.title);
      alert(my_data.desc);
    },
  },
};
</script>