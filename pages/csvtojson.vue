<template>
  <!DOCTYPE html>
  <html lang="en">
    <head>
      <meta charset="UTF-8" />
      <meta name="viewport" content="width=device-width, initial-scale=1.0" />
      <title>Document</title>
    </head>
    <body>
      <div class="page">
        <input v-model="name" />
        <ul>
          <li v-for="i in fInfo" :key="i.id">
            {{ i }}
          </li>
        </ul>
      </div>
    </body>
  </html>
</template>

<script>
import axios from 'axios'
export default {
  data() {
    return {
      info: [],
      name: '',
    }
  },
  computed: {
    fInfo() {
      return this.info.filter((e) => {
        return e.title.indexOf(this.name) != -1
      })
    },
  },
  mounted() {
    axios
      .get('https://jsonplaceholder.typicode.com/posts/')
      .then((response) => (this.info = response.data))
  },
}
</script>
