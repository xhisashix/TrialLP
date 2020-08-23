<template lang="pug">
  .airrelief
    Airtitle(title="万一のときも安心です")
    .content
      .content-text
        p 大切なお家にお迎えする相手選びは、信頼第一で進めたいですよね。 その思いに応えるため、Airbnbでは宿泊者に求める厳格な要件をホスト自身の手で設定し、滞在前にお互い交流できるシステムを採用しています。 万一のトラブルのときには、Airbnbが全力でサポートします。 建物・家財の被害は「ホスト保証」、賠償責任は「ホスト補償保険」でカバー。ホストのみなさまのあらゆるシチュエーションに対処しています。
        a(href="#") ホストを守るAirbnbの仕組みをチェック
      .content-list
        ul
          li(v-for="l in items") {{ l.item }}
    img(src="https://a0.muscache.com/pictures/bb358a46-fa25-4895-b5fd-048a386bdcac.jpg")
</template>

<script>
export default {
  data() {
    return {
      items: [
        { item: '予約前に政府発行の身分証明書を求める権限' },
        { item: 'ハウスルールに同意しないと泊まれない' },
        { item: '財物損害は¥100,000,000まで無料で補償' },
        { item: '$1,000,000の賠償責任保険が無料で付帯' },
        { item: '24時間365日対応グローバルカスタマーサポート' },
      ],
    }
  },
}
</script>

<style lang="stylus">
.airrelief
  width 70%
  margin 0 auto

  .content
    display flex

    .content-text
      flex 1

      a
        color #16a085
        display flex
        margin-top 30px
    .content-list
      flex 1
      margin-left 80px
      display flex
      align-items center
      ul
        list-style-type none
        margin 0 auto
        li
          position relative
          margin-bottom 20px
          &afte
            content ''
            display block
            position absolute
            top 0.3em
            left -1.7em
            width 20px
            height 10px
            border-left 2px solid #16a085
            border-bottom 2px solid #16a085
            transform rotate(-45deg)
  img
    display flex
    margin 0 auto
    margin-top 30px
    width 1000px
    height 600px
</style>