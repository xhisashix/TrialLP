<template lang="pug">
  .airmv
    .form
      h1 Airbnbホストになって、暮らしをレベルアップ
      p 宿泊施設の内容を記入
      form
        input(type="text" placeholder="name")
        .choose
          select
            option まるまる貸し切り
            option 個室
            option シェアルーム
          select
            option ゲスト4人
            option ゲスト3人
            option ゲスト2人
        .mvbutton
          Airbutton
</template>

<script>
import Airbutton from '~/components/airbnb/Airbutton'
export default {
  Airbutton,
}
</script>

<style lang="stylus">
.airmv {
  background-image: url('https://images.unsplash.com/photo-1470110385011-8c66cb46f0e9?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=500&q=60');
  background-size: cover;
  height: 70vh;
  position: relative;

  .form {
    background: #ffffff;
    width: 25vw;
    height: 400px;
    position: absolute;
    top: 20%;
    left: 60%;
    padding: 10px;

    form {
      display: flex;
      flex-direction: column;
      width: 100%;
      margin: 0 auto;

      input {
        height: 50px;
        padding: 8px;
        font-size: 20px;
        margin-top: 10px;
      }

      .choose {
        display: flex;
        margin-top: 5px;

        select {
          flex: 1;
          margin-right: 10px;
          height: 50px;
          font-size: 20px;
        }
      }

      .mvbutton {
        margin-top: 30px;
      }
    }
  }
}
</style>