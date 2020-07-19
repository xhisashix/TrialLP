<template lang="pug">
.contact
  HLTitle(title='Contact' :white='true')
  .contact-box
    p お気軽にご相談ください。
    Button(button='Contact')
  Our(our='Contact us' :left='true')
</template>
<script>

import HLTitle from '~/components/ui/HLTitle'
import Our from '~/components/ui/Our'
import Button from '~/components/ui/Button'
export default {
  components:{
    HLTitle,
    Our,
    Button
  },
}
</script>
<style lang="stylus">
.contact {
  padding-top: 30px;
  margin-top: 120px;
  background: rgba(0 0 0 0.7);
  text-align: center;

  p {
    margin-top: 80px;
    color: #ffffff;
    font-size: 20px;
    font-weight: bold;
  }
}
</style>