<template>
  <div class="page">

    <div class="page__hd">
      <div class="page__title">Switch</div>
      <div class="page__desc">开关项</div>
    </div>

    <div class="page__bd">
      <div class="weui-cells__title">开关项</div>
      <div class="weui-cells weui-cells_after-title">
        <ui-switch label="标题文字" @change="change" />
        <ui-switch label="标题文字" color="red" @change="change" checked />
      </div>
    </div>

  </div>
</template>

<script>
import uiSwitch from '../../../components/switch'

export default {
  components: {
    uiSwitch,
  },

  methods: {
    change (checked) {
      console.log(`switch 值：${checked}`)
    },
  },
}
</script>

<style>
</style>
