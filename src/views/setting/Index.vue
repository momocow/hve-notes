<template>
  <div class="">
    <v-tabs
      v-model="active"
      color="#1067de"
      dark
      slider-color="white"
    >
      <v-tab ripple>️️️⚙️ 基础配置</v-tab>
      <v-tab ripple>💬 GITALK 配置</v-tab>
      <v-tab ripple>🌅 FAVICON</v-tab>
      <v-tab-item>
        <basic-setting></basic-setting>
      </v-tab-item>
      <v-tab-item>
        <gitalk-setting></gitalk-setting>
      </v-tab-item>
      <v-tab-item>
        <favicon-setting></favicon-setting>
      </v-tab-item>
    </v-tabs>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import Component from 'vue-class-component'
import BasicSetting from './includes/BasicSetting.vue'
import GitalkSetting from './includes/GitalkSetting.vue'
import FaviconSetting from './includes/FaviconSetting.vue'

@Component({
  components: {
    BasicSetting,
    GitalkSetting,
    FaviconSetting,
  },
})
export default class Setting extends Vue {
  active = null
}
</script>

<style lang="stylus" scoped>
</style>
