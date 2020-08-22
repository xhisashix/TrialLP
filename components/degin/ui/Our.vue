<template lang="pug">
  .our(:class="{ left : left}")
    h1 {{ our }}
</template>
<script>
export default {
  props:{
    our:{
      type : String,
      default: 'Our'
    },
    left:{
      type: Boolean,
      default: false
    }
  }
}
</script>
<style lang="stylus">
.our {
  font-size: 70px;
  font-weight: bold;
  opacity: 0.05;
  font-family: serif;
  text-align: right;
  margin-right: 120px;

  &.left {
    text-align: left;
    margin-left: 120px;
  }
}
</style>