<template>
  <div>
    <div class="dialog">
      <el-button @click="visible = true">ダイヤログを開く</el-button>
      <el-dialog :visible.sync="visible" title="確認">
        <p>testtest</p>
      </el-dialog>
    </div>
    <div class="switch">
      <el-switch v-model="value1" disabled> </el-switch>
      <el-switch
        v-model="value2"
        active-color="#13ce66"
        inactive-color="#ff4949"
      >
      </el-switch>
    </div>
    <div class="slider">
      <div class="block">
        <el-slider v-model="value" show-input> </el-slider>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data: function () {
    return {
      visible: false,
      value1: true,
      value2: true,
      value: 0,
    }
  },
}
</script>

<style lang="stylus">
.dialog
  margin-left 20px
  margin-top 20px
.switch
  margin-left 20px
  margin-top 20px
.slider
  widows 90%
  margin-left 20px
  margin-top 20px
</style>
