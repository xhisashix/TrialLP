<template lang="pug">
.concept
  HLTitle(title='CONCEPT')
  h3 “働きたくなる空間”をデザインすることで<br>人々を幸せにする。
  .content-box
    p 私たちは、オフィスに特化した空間デザイン専門としております。その理由は、「働きたくなる空間で仕事ができれば多くの人を幸せにできるのではないか」と考えるためです。そんな想いの株式会社Cresta Designだからこそできる空間デザインを提供させていただきます。
    img(src="img/concept-image.png")
  Our(our='Our Concept')
</template>

<script>
import HLTitle from '~/components/degin/ui/HLTitle'
import Our from '~/components/degin/ui/Our'
export default {
  components: {
    HLTitle,
    Our,
  },
}
</script>
<style lang="stylus">
.concept {
  display: block;
  margin-top: 120px;

  h3 {
    text-align: center;
    margin-top: 70px;
  }

  .content-box {
    display: flex;
    margin: 60px 220px 70px;

    img {
      margin-left: 120px;
    }

    p {
      display: flex;
      align-items: center;
    }
  }
}
</style>