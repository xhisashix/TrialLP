<template lang="pug">
  .airclearing
    Airtitle(title="シンプルな決済")
    .content
      ul
        li(v-for="l in items")
          h2 {{ l.title}}
          p {{ l.text }}
    a(href="#") Airbnb収入を得るまでの流れを見る
</template>

<script>
export default {
  data() {
    return {
      items: [
        {
          title: '料金設定は完全に自由',
          text:
            '料金は常に自由に選択できます。 迷ったときには、 域内需要に合わせて設定できるツールがあります。',
        },
        {
          title: '手数料が安い',
          text:
            '登録に費用は一切かかりません。Airbnbは通常、予約ごとに業界で最低の均一3％をサービス料としていただいております。',
        },
        {
          title: '迅速な支払い',
          text:
            'ゲストのチェックイン後に、Paypal、直接振り込み、またはその他の利用可能な方法で受取金を送金できます。',
        },
      ],
    }
  },
}
</script>

<style lang="stylus">
.airclearing {
  width: 80%;
  margin: 0 auto;

  .content {
    ul {
      display: flex;
      list-style: none;
      width: 100%;
      margin: 0 auto;
      justify-content: space-between;

      li {
        line-height: 2;
        margin: 0 30px;
      }
    }
  }

  a {
    display: flex;
    justify-content: flex-end;
    margin-right: 100px;
    margin-top: 20px;
    color: #16a085;
  }
}
</style>