<template lang="pug">
  .airfooter
    ul
      li
        h3 企業情報
        p Airbnbのご利用方法
        p ニュースルーム
        p Airbnb Citizen
        p Airbnb Plus
        p Airbnb Luxe
        p HotelTonight
        p Airbnbビジネスプログラム
        p オリンピック
        p 採用情報
      li
        h3 コミュニティ
        p ダイバーシティ＆ビロンギング
        p アクセシビリティ対応
        p Airbnb Magazine
        p Airbnbアソシエイト
        p お友達を招待
      li
        h3 ホスト
        p お部屋を掲載
        p オンライン体験をホストする
        p 体験をホストする
        p CEOブライアン・チェスキーからのメッセージ
        p 責任あるホスティング
        p オープンホーム
        p リソースセンター
        p コミュニティセンター
      li
        h3 サポート
        p 新型コロナウイルスに関する最新情報
        p ヘルプセンター
        p キャンセルオプション
        p 近隣コミュニティサポート
        p 信頼＆安全
    .conpany
      .content
        a(href="#") Airbnb Global Services Limited
        a(href="#") 観光庁長官(01)第S0001号(2018年6月15日-2023年6月14日)
        p © 2020 Airbnb, Inc. All rights reserved·プライバシー·利用規約·サイトマップ·企業情報
</template>

<script>
export default {}
</script>

<style lang="stylus">
.airfooter {
  width: 100%;
  background: #ecf0f1;
  margin-top: 50px;
  padding: 20px;

  ul {
    width: 90%;
    margin: 0 auto;
    list-style: none;
    margin-top: 40px;
    display: flex;
    justify-content: space-between;
    font-size: 12px;

    li {
      p {
        margin-top: 10px;
      }
    }
  }

  .conpany {
    width: 90%;
    margin: 0 auto;
    margin-top: 30px;
    border-top: 1px solid #000;

    .content {
      height: 15vh;
      display: flex;
      flex-direction: column;
      justify-content: center;
    }
  }
}
</style>