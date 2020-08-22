<template lang="pug">
  .airheader
    img(src="#" alt="logoが入るよ")
    ul
      li
        a(href="#") 概要
      li
        a(href="#") 準備
      li
        a(href="#") 安全
      li
        a(href="#") マネープラン
    .headerbutton
      .button
        Airbutton
</template>

<script>
import Airbutton from '~/components/airbnb/Airbutton'
export default {
  Airbutton,
}
</script>

<style lang="stylus">
.airheader {
  display: flex;
  height: 60px;
  position: fixed;
  z-index: 1;
  width: 100%;
  background-color: #f5f6fa;

  ul {
    display: flex;
    flex: 1;
    margin-left: 20px;
    list-style: none;
    align-items: center;
    font-weight: bold;

    li {
      margin-left: 30px;

      &:hover {
        border-bottom: 1px solid #00b894;
      }
    }
  }

  .headerbutton {
    flex: 1;
    height: 60px;
    margin: auto 0;
    display: flex;
    align-items: center;
    justify-content: flex-end;
    margin-right: 30px;

    .button {
      justify-content: flex-end;
      display: flex;
      align-items: center;
    }
  }
}
</style>