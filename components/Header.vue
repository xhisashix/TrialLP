<template lang="pug">
.header
  Slidshow
  header
    h1 Cresta Design
    ul: li(v-for="item in items") {{ item.list }}
    .top-text
      h2 Design for Smile.
      p 快適なオフィスをデザインする
</template>
<script>
export default {
  data () {
    return {
      items: [
        { list: 'Concept' },
        { list: 'Service' },
        { list: 'Work' },
        { list: 'Contact' }
      ]
    }
  },
  computed: {
  },
  methods: {
  }
}
</script>
<style lang="stylus">
.header {
  position: relative;

  img {
    width: 100%;
  }

  header {
    font-family: serif;
    width: 100%;
    display: flex;
    position: absolute;
    top: 0;
    left: 0;
    padding: 20px 120px;
    color: #ffffff;
    align-items: center;

    h1 {
      flex: 1;
      font-size: 26px;
      font-weight: bold;
    }

    ul {
      display: flex;
      list-style: none;
      justify-content: flex-end;

      li {
        margin-left: 20px;
        font-size: 16px;
        font-weight: bold;
      }
    }

    .top-text {
      position: absolute;
      left: 120px;
      top: 409px;

      h2 {
        font-size: 70px;
        font-weight: bold;
      }

      p {
        font-size: 40px;
        font-weight: bold;
      }
    }
  }
}
</style>