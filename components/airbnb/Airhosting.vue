<template lang="pug">
  .airhosting
    Airtitle(title="3ステップでホスティング")
    .hostingcontent
      ul: li(v-for="item in items")
        h2 {{ item.list }}
        p {{ item.text }}
      .checklink
        a(href="#", title="title") ホストをはじめる方法をチェック
</template>

<script>
export default {
  data() {
    return {
      items: [
        {
          list: '無料でお部屋を掲載',
          text:
            '共有のリビングルームから別荘に至るまで、どんなスペースでも登録料なしで共有しましょう。',
        },
        {
          list: 'ホスティング方法を設定',
          text:
            'スケジュール、料金、ゲストへの要件をご自身で選択しましょう。 お困りの際にはいつでもサポートいたします。',
        },
        {
          list: 'はじめてのゲストが来ます！',
          text:
            'リスティングが掲載されると、条件にかなったゲストから連絡を受けとることができます。 ゲストの到着前に質問があればメッセージを送信できます。',
        },
      ],
    }
  },
}
</script>
<style lang="stylus">
.airhosting
  ul
    margin: 0 auto;
    margin-top: 50px;
    display: flex;
    list-style: none;
    width: 70%;
    line-height: 1.5;
    li
      margin-left: 50px;
      h2
        font-size: 28px;

  .checklink
    width: 70%;
    margin: 0 auto;
    margin-top: 20px;
    a
      display: flex;
      justify-content: flex-end;
      margin-right: 15px;
</style>