<template lang="pug">
.air-practice-sample
  img(src="https://a0.muscache.com/pictures/4e8524b4-205e-4fdf-9f0a-f1f36905c8f6.jpg")
  .content
    h1 ❝
    h3 ホスト収入でキッチンリフォーム。お家をいろいろアップグレードしました。
    p Tessaさんはロンドン在住。ホストになって経済的なゆとりができました
    a(href="#") ホスト実践例をチェック
</template>

<script>
export default {}
</script>

<style lang="stylus">
.air-practice-sample {
  display: flex;
  width: 80%;
  margin: 0 auto;
  margin-top: 50px;

  img {
    width: 500px;
    height: 500px;
  }

  .content {
    margin-left: 80px;
    width: 40%;
    display: flex;
    justify-content: center;
    flex-direction: column;

    h1 {
      font-size: 48px;
      color: #f1c40f;
    }

    h3 {
      margin-top: 10px;
      font-size: 30px;
      font-weight: normal;
      line-height: 1.2;
    }

    p {
      margin-top: 20px;
    }

    a {
      text-align: center;
      border: 2px solid #000;
      padding: 10px;
      border-radius: 5px;
      box-sizing: content-box;
      margin-top: 20px;
      display: flex;
      align-items: center;
      justify-content: center;
      width: 200px;
      text-decoration: none;
      color: #000;
    }
  }
}
</style>