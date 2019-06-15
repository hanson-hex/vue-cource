<template>
  <div id="app">
    <ol>
      <todo-item v-for="item in groceryList" v-bind:todo="item" v-bind:key="item.id" ></todo-item>
    </ol>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import TodoItem from './components/TodoItem.vue'

export default {
    name: 'app',
    components: {
        TodoItem
    },
    data() {
        return {
            groceryList: [
                {
                    id: 0,
                    text: 'cl'
                },
                {
                    id: 1,
                    text: 'nai'
                }]
        }
    }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
