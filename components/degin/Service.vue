<template lang="pug">
.service
  HLTitle(title='Service')
  .img-box
    ul
      li
        img(src="img/service-img01.png")
        p Hearing
      li
        img(src="img/service-img02.png")
        p Planning
      li
        img(src="img/sevice-img03.png")
        p Direction
  Our(our='Our Service')
</template>
<script>

import HLTitle from '~/components/degin/ui/HLTitle'
import Our from '~/components/degin/ui/Our'
export default {
  components:{
    HLTitle,
    Our
  },
}
</script>
<style lang="stylus">
.img-box {
  ul {
    display: flex;
    margin: 0;
    padding: 0;
    list-style: none;
    display: inline-flexbox;
    height: 320px;
    margin-top: 80px;

    li {
      position: relative;
      flex: 1;

      img {
        position: absolute;
      }

      img:hover {
        background: black;
        opacity: 0.8;
      }

      p {
        position: absolute;
        z-index: 100;
        display: flex;
        justify-content: center;
        align-items: center;
        top: 148px;
        left: 132px;
        font-size: 40px;
        font-weight: bold;
        color: #ffffff;
        font-family: serif;
      }
    }
  }
}
</style>