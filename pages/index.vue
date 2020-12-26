<template lang="pug">
  .indexTitle
    h1 下記のリンクから別ページへ
    .link
      a(href="airbnb") airbnbページへ
      a(href="degin") deginページへ
      a(href="csvtojson") csvtojsonページへ
      a(href="todo") todoページへ
      a(href="element") elementページへ
      a(href="calendar") calendarページへ
</template>
<script>
export default {}
</script>
<style lang="stylus">
.indexTitle
  width 100%
  h1
    text-align center
.link
  margin-top 20px
  display flex
  justify-content center
  align-items center
  a
    border 1px solid #000
    width 200px
    margin-top 20px
    text-align center
    margin-left 20px
    text-decoration none
    color #ffffff
    background-color #000
</style>
