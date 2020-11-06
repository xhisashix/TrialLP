<template>
  <div id="app" class="container">
    <h1>
      My Todos
      <span class="info">({{ remaining.length }}/{{ todos.length }})</span>
    </h1>
    <ul>
      <li v-for="(todo, index) in todos" :key="index">
        <input type="checkbox" v-model="todo.isDone" name="" id="" />
        <span :class="{ done: todo.isDone }">{{ todo.title }}</span>
        <span @click="deleteItem(index)" class="command"> × </span>
      </li>
      <li v-show="!todos.length">タスクなし</li>
    </ul>

    <form @submit.prevent="addItem">
      <input type="text" v-model="newItem" />
      <input type="submit" value="Add" />
      <div class="todo-delete">
        <button @click="purge">削除</button>
      </div>
    </form>
  </div>
</template>
<script>
export default {
  data() {
    return {
      newItem: '',
      todos: [],
    }
  },
  watch: {
    todos: function () {
      handler: {
        localStorage.setItem('todos', JSON.stringify(this.todos))
      }
      deep: true
    },
  },
  mounted: function () {
    this.todos = JSON.parse(localStorage.getItem('todos')) || []
  },
  methods: {
    addItem: function () {
      var item = {
        title: this.newItem,
        isDone: false,
      }
      this.todos.push(item)
      this.newItem = ''
    },
    deleteItem: function (index) {
      if (confirm('このタスクをに消しますか')) {
        this.todos.splice(index, 1)
      }
    },
    purge: function () {
      if (!confirm('完了したタスクを削除しますか')) {
        return
      }
      this.todos = this.remaining
    },
  },
  computed: {
    remaining: function () {
      return this.todos.filter(function (todo) {
        return !todo.isDone
      })
    },
  },
}
</script>

<style>
.container {
  width: 300px;
  margin: 0 auto;
}

#app h1 {
  font-size: 16px;
  border-bottom: 1px solid #ddd;
  padding: 16px 0;
}

#app li {
  line-height: 1.5;
  margin: 5px 0;
}

#app input[type='text'] {
  padding: 2px;
}

.command {
  font-size: 24px;
  cursor: pointer;
  color: #08c;
}

#app ul {
  padding: 0;
  list-style: none;
}

#app li > span.done {
  text-decoration: line-through;
  color: #bbb;
}

.info {
  color: #bbb;
  font-size: 12px;
  font-weight: normal;
}

#app h1 > button {
  float: right;
}

.todo-delete > button {
  height: 20px;
  border: #000 solid 1px;
  background: #ffffff;
  border-radius: 0;
  margin: 10px;
}
</style>
