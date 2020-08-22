<template lang="pug">
  .title(:class="{white : white}")
    h1 {{ title }}
</template>

<script>
export default {
  props:{
    title:{
      default:'タイトル',
      type: String
    },
    white:{
      type: Boolean,
      default: false
    }
  }
}
</script>

<style lang="stylus">
.title {
  display: flex;
  align-items: center; /* 垂直中心 */
  justify-content: flex-start; /* 水平中心 */
  color: #000000;
  margin-left: 220px;
  margin-top: 100px;

  &.white {
    justify-content: flex-end;
    color: #ffffff;
    margin-right: 220px;
  }

  h1 {
    font-size: 60px;
    font-family: serif;
  }
}

.title:after {
  border-top: 5px solid;
  content: '';
  width: 200px; /* 線の長さ */
}

.title:after {
  margin-left: 1em; /* 文字の左隣 */
}
</style>