<template>
  <fm-tab-page :tab-titles="tabTitles"
                ref="fm-tab-page">
    <list v-for="(v, index) in tabTitles" :key="index"
          :slot="`tab-item-${index}`"
          class="item-container">
      <cell v-for="(item, idx) in listData" :key="idx">
        <fm-pan-item @fmPanItemPan="fmPanItemPan">
          <text class="cell">{{ item }}</text>
        </fm-pan-item>
      </cell>
    </list>
  </fm-tab-page>
</template>

<style scoped>
  .item-container {
    width: 1080px;
  }

  .cell {
    border-bottom-width: 1px;
    height: 144px;
  }
</style>

<script>
  import { FmTabPage, FmPanItem, BindEnv } from 'weex-flymeui'

  export default {
    components: { FmTabPage, FmPanItem },
    data () {
      return {
        tabTitles: [{
          title: '标签1'
        }, {
          title: '标签标签',
          selected: false
        }, {
          title: 'NBA'
        }, {
          title: '超长的标签啊啊啊'
        }, {
          title: '标签'
        }],
        listData: ['哈哈哈', '哈哈', '哈哈', '哈哈', '哈哈', '哈哈', '哈哈', '哈哈', '哈哈', '哈哈', '哈哈', '哈哈', '哈哈', '哈哈', '哈哈', '哈哈', '哈哈', '哈哈', '哈哈', '哈哈'],
        select: 1
      }
    },
    methods: {
      fmPanItemPan (e) {
        if (BindEnv.supportsEBForAndroid()) {
          this.$refs['fm-tab-page'].bindExp(e.element)
        }
      }
    },
    mounted () {
      setTimeout(() => {
        this.tabTitles.push({ title: '12312' })
      // console.log(this.tabTitles);
      })
    }
  }
</script>
