<template lang="pug">
.work
  HLTitle(title='Works' :white='true')
  .content-box
    ul
      li
        img(src="img/card-img01.png")
        p 新規サイトを公開しました。今回のサイトは白と黒を基調にしたミニマルなデザインになっています。
      li
        img(src="img/card-img02.png")
        p 新規サイトを公開しました。今回のサイトは白と黒を基調にした
      li
        img(src="img/card-img03.png")
        p 新規サイトを公開しました。今回のサイトは白と黒を基調にしたミニマルなデザインになっています。
    Button(button="View More")
  Our(our='Our Works' :left='true')
</template>
<script>
import HLTitle from '~/components/degin/ui/HLTitle'
import Our from '~/components/degin/ui/Our'
import Button from '~/components/degin/ui/Button'
export default {
  components: {
    HLTitle,
    Our,
    Button,
  },
}
</script>
<style lang="stylus">
.work {
  padding-top: 100px;
  background-color: rgba(0 0 0 0.7);

  ul {
    margin-top: 80px;
    display: flex;
    list-style: none;
    margin: 80px 220px 0;
    justify-content: center;

    li {
      display: flex;
      flex: 1;
      flex-direction: column;
      background-color: #ffffff;
      margin-left: 20px;

      p {
        padding: 20px;
        line-height: 30px;
      }
    }
  }
}
</style>