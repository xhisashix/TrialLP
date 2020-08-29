<template lang="pug">
  .airquestion
    Airtitle(title="よくある質問")
    .box
      .content
        a(href="#") Airbnbホストになれるのはどんな人？
        a(href="#") 予約前にゲストに求められる要件は？
        a(href="#") お部屋の掲載料はいくら？
      .content
        a(href="#") 家財破損があった場合、どのような補償がありますか？
        a(href="#") リスティングの料金を選ぶには？
        a(href="#") 料金設定の支援ツールはありますか？
    .airdetail
      h3 ホスティングの詳細はこちら
      ul
        li(v-for="l in items")
          img(src="https://a0.muscache.com/pictures/489faa5d-9519-48fa-aa0e-fe9673165e43.jpg")
          p {{ l.title }}
          p {{ l.text }}
          a(href="#") もっと詳しく見る

    .monetization
      h1 収益化試して<br>みませんか
      a(href="#") はじめる
</template>

<script>
export default {
  data() {
    return {
      items: [
        {
          title: '初期設定',
          text: 'ホスティング入門',
        },
        {
          title: '初期設定',
          text: 'ホスティング入門',
        },
        {
          title: '初期設定',
          text: 'ホスティング入門',
        },
      ],
    }
  },
}
</script>

<style lang="stylus">
.airquestion
  .box
    display flex
    width 80%
    margin 0 auto
    .content
      flex 1
      display flex
      flex-direction column
      margin-left 10px
      a
        padding 30px 0
        color #00b894
        border-bottom 1px solid #000000
  .airdetail
    width 70%
    margin 0 auto
    margin-top 50px
    ul
      display flex
      list-style none
      li
        margin-left 20px
        img
          width 100%
  .monetization
    width 70%
    height 400px
    margin 0 auto
    margin-top 50px
    background-image url("https://images.unsplash.com/photo-1526970498195-e45b3ea092b1?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=500&q=60")
    object-fit cover
    background-size cover
    padding 30px
    h1
      font-size 4rem
      color #fff
    a
      background #fff
      color #000
      display flex
      justify-content center
      align-items center
      height 50px
      width 200px
      border-radius 10px
</style>
