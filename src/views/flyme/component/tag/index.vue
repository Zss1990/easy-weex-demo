<template>
  <div class="mzui-demo">
    <scroller class="scroller">
      <title link="https://yanjiie.github.io/weex-flymeui/#/packages/fm-tag/"></title>
      <category title="小标签"></category>
      <div class="cell">
        <fm-tag value="新手上asdas路"></fm-tag>
        <fm-tag value="热asd映" color="#f12528"></fm-tag>
        <fm-tag value="票asdsa" color="#ffaf00"></fm-tag>
        <fm-tag value="新手上路asdasd"></fm-tag>
        <fm-tag value="热映" color="#f12528"></fm-tag>
        <fm-tag value="票" color="#ffaf00"></fm-tag>
        <fm-tag value="新手fad上路"></fm-tag>
        <fm-tag value="热asdsa映" color="#f12528"></fm-tag>
        <fm-tag value="票" color="#ffaf00"></fm-tag>
        <fm-tag value="新手asdasd上路"></fm-tag>
        <fm-tag value="热asdfasdfadsfdsfadsfdsafads映" color="#f12528"></fm-tag>
        <fm-tag value="票" color="#ffaf00"></fm-tag>
        <fm-tag value="热fsdafa映" color="#f12528"></fm-tag>
        <fm-tag value="asdfsaddfs票" color="#ffaf00"></fm-tag>
        <fm-tag value="新asfgasfgs手上路"></fm-tag>
        <fm-tag value="热映" color="#f12528"></fm-tag>
        <fm-tag value="票" color="#ffaf00"></fm-tag>
        <fm-tag value="新asgasgaswg手上路"></fm-tag>
        <fm-tag value="热映" color="#f12528"></fm-tag>
        <fm-tag value="票" color="#ffaf00"></fm-tag>
        <fm-tag value="新asdfasdfdas手上路"></fm-tag>
        <fm-tag value="热映" color="#f12528"></fm-tag>
        <fm-tag value="票" color="#ffaf00"></fm-tag>
        <fm-tag value="新手asdfasdfadsfads上路"></fm-tag>
        <fm-tag value="热映" color="#f12528"></fm-tag>
        <fm-tag value="热映" color="#f12528"></fm-tag>
        <fm-tag value="票" color="#ffaf00"></fm-tag>
        <fm-tag value="新手上路"></fm-tag>
        <fm-tag value="热映" color="#f12528"></fm-tag>
        <fm-tag value="票" color="#ffaf00"></fm-tag>
        <fm-tag value="新手上路"></fm-tag>
        <fm-tag value="新手上路"></fm-tag>
        <fm-tag value="热映" color="#f12528"></fm-tag>
        <fm-tag value="票" color="#ffaf00"></fm-tag>
        <fm-tag value="新手上路"></fm-tag>
        <fm-tag value="票" color="#ffaf00"></fm-tag>
        <fm-tag value="新手上路"></fm-tag>
        <fm-tag value="热映" color="#f12528"></fm-tag>
        <fm-tag value="票" color="#ffaf00"></fm-tag>
      </div>
      <category title="大标签"></category>
      <div class="cell">
          <fm-tag value="HQ" size="big" color="#f12528"></fm-tag>
          <fm-tag value="热映" size="big" color="#ffaf00"></fm-tag>
          <fm-tag value="票" size="big" color="#3bc06b"></fm-tag>
      </div>
      <category title="腰圆标签"></category>
      <div class="cell">
          <fm-tag value="腰圆标签" size="huge" color="#f12528"></fm-tag>
          <fm-tag value="推荐" size="huge" color="#ffaf00"></fm-tag>
          <fm-tag value="你给我听好" size="huge" color="#3bc06b"></fm-tag>
      </div>
      <category title="空心标签"></category>
      <div class="cell">
          <fm-tag value="HQ" size="big" type="hollow" color="#f12528" fontColor="#3bc06b"></fm-tag>
          <fm-tag value="热映" size="big" type="hollow" color="#ffaf00" fontColor="#f12528"></fm-tag>
          <fm-tag value="票" size="big" type="hollow" color="#3bc06b" fontColor="#3bc06b"></fm-tag>
      </div>
    </scroller>
  </div>
</template>

<style scoped>
  .mzui-demo {
    position: absolute;
    top: 0;
    right: 0;
    left: 0;
    bottom: 0;
    background-color: #ffffff;
  }

  .cell {
    padding: 45px;
    flex-direction: row;
    align-items: flex-start;
    flex-wrap: wrap;
  }

  .scroller {
    position: absolute;
    top: 0;
    right: 0;
    left: 0;
    bottom: 0;
  }
</style>

<script>
  import { FmTag } from 'weex-flymeui'
  import Title from '@components/flyme/_mods/title.vue'
  import Category from '@components/flyme/_mods/category.vue'

  export default {
    components: { Title, Category, FmTag }
  }
</script>
