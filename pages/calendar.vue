<template lang="pug">
.Ctitle
  h1 calendar

  .calendar
    table
      tr
        th(v-for="week in weeks") {{ week }}
  .now
    p {{ time() }}

</template>

<script>
export default {
  data() {
    return {
      weeks: ['日', '月', '火', '水', '木', '金', '土'],
      d: 0,
      now: '',
    }
  },
  methods: {
    time: function (e) {
      var date = new Date()
      return (this.now = date.getDate())
    },
  },
}
</script>

<style lang="stylus"></style>
