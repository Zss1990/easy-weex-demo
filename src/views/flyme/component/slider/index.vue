<template>
  <scroller class="wrap">
    <title link="https://yanjiie.github.io/weex-flymeui/#/packages/fm-slider/"></title>
    <category title="基本使用"></category>
    <fm-slider :items="items" :auto-play="true"></fm-slider>
  </scroller>
</template>

<style scoped>
  .wrap {
    position: absolute;
    top: 0;
    right: 0;
    left: 0;
    bottom: 0;
  }
</style>

<script>
  import { FmSlider, FmButton, FmText, FmFooter } from 'weex-flymeui'
  import Title from '@components/flyme/_mods/title.vue'
  import Category from '@components/flyme/_mods/category.vue'
  export default {
    components: { Title, Category, FmSlider, FmButton, FmText, FmFooter },
    data: () => ({
      page: 0,
      items: [
        {
          src: 'http://gw.alicdn.com/imgextra/i4/169/TB2TlW1aLuSBuNkHFqDXXXfhVXa_!!169-0-lubanu.jpg_q50.jpg'
        },
        {
          src: 'http://gw.alicdn.com/imgextra/TB2nu8oev5TBuNjSspcXXbnGFXa_!!103-0-lubanu.jpg_q50.jpg'
        },
        {
          src: 'http://gw.alicdn.com/imgextra/TB2dprKdFuWBuNjSszbXXcS7FXa_!!124-0-luban.jpg_q50.jpg'
        },
        {
          src: 'http://img.alicdn.com/imgextra/i4/18/TB28vYEdL9TBuNjy0FcXXbeiFXa_!!18-0-luban.jpg_q50.jpg'
        },
        {
          src: 'http://aecpm.alicdn.com/simba/img/TB14ab1KpXXXXclXFXXSutbFXXX.jpg_q50.jpg'
        }
      ]
    }),
    methods: {
      prev () {
        this.$refs.banner.prev()
      },
      next () {
        this.$refs.banner.next()
      }
    }
  }
</script>
