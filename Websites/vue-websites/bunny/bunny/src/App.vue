<template>
  <div>
    <Todos v-bind:todos="todos"/>
  </div>
</template>

<script>
import Todos from "./components/Todos";

export default {
  name: 'App',
  components: {
    Todos
  },
  data() {
    return {
      todos:[
        {
          id: 1,
          title:"Todo one",
          completed: false
        },
        {
          id: 2,
          title:"Todo two",
          completed: true
        },
        {
          id: 1,
          title:"Todo three",
          completed: false
        },
      ]
    }
  }
}
</script>

<style>
  * {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
  }
  body {
    font-family:'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
    line-height: 1.4;
  }
</style>
