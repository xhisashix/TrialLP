<template lang="pug">
  .btn
      button {{ button}}
</template>

<script>
export default {
  props:{
    button:{
      type: String,
      default: 'button'
    }
  }
}
</script>

<style lang="stylus">
button {
  height: 59px;
  width: 235px;
  background: #F7D43F;
  display: flex;
  justify-content: center;
  align-items: center;
  margin: 80px auto;
  border-radius: 50px;
  font-weight: bold;
  font-family: serif;
  border: none;
}
</style>