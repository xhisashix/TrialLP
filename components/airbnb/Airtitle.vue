<template lang="pug">
  .airtitle
    h1
      span {{ title }}
</template>

<script>
export default {
  props: {
    title: {
      type: String,
      default: 'Title',
    },
  },
}
</script>

<style lang="stylus">
.airtitle
  margin-top 80px

  h1
    position relative
    padding 1.5rem
    text-align center
    font-size 48px
    &:before
      position absolute
      top 10px
      left calc(50% - 30px)
      width 100px
      height 1px
      content ''
      border-radius 3px
      background #000
</style>