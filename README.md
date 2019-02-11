# WoopDogg
&lt;template>   &lt;d2-container :filename="filename" class="page">     &lt;d2-page-cover>       &lt;d2-icon-svg         class="page__logo"         name="d2-admin"/>       &lt;template slot="footer">         &lt;div class="page__btn-group">           &lt;span @click="$open('https://github.com/d2-projects')">开源组织&lt;/span> |           &lt;span @click="$open('https://doc.d2admin.fairyever.com/zh/')">文档&lt;/span> |           &lt;span @click="$open('https://github.com/d2-projects/d2-admin-start-kit')">简化版&lt;/span> |           &lt;span @click="$open('https://alibaba.github.io/ice/scaffold?type=vue')">飞冰&lt;/span> |           &lt;span @click="$open('https://juejin.im/user/57a48b632e958a006691b946/posts')">掘金&lt;/span> |           &lt;span @click="$open('https://awesome.fairyever.com/daily/')">开发者日报&lt;/span> |           &lt;el-popover             :width="172"             trigger="hover">             &lt;p class="d2-mt-0 d2-mb-10">D2Projects&lt;/p>             &lt;img               src="./image/qr@2x.png"               style="width: 172px;">             &lt;span slot="reference">微信公众号&lt;/span>             &lt;p style="font-size: 12px; margin-top: 0px; margin-bottom: 0px;">               官方公众号，主要推送前端技术类文章、框架资源、学习教程，以及 D2 系列项目更新信息             &lt;/p>           &lt;/el-popover>         &lt;/div>         &lt;d2-badge/>         &lt;d2-help-btn/>       &lt;/template>     &lt;/d2-page-cover>   &lt;/d2-container> &lt;/template>  &lt;script> import D2HelpBtn from './components/d2-help-btn' import D2Badge from './components/d2-badge' export default {   components: {     D2HelpBtn,     D2Badge   },   data () {     return {       filename: __filename     }   } } &lt;/script>  &lt;style lang="scss" scoped> .page {   .page__logo {     width: 120px;   }   .page__btn-group {     color: $color-text-placehoder;     font-size: 12px;     margin-top: 0px;     margin-bottom: 20px;     span {       color: $color-text-sub;       &amp;:hover {         color: $color-text-main;       }     }   } } &lt;/style>
<template>
  <d2-container :filename="filename" class="page">
    <d2-page-cover>
      <d2-icon-svg
        class="page__logo"
        name="d2-admin"/>
      <template slot="footer">
        <div class="page__btn-group">
          <span @click="$open('https://github.com/d2-projects')">开源组织</span> |
          <span @click="$open('https://doc.d2admin.fairyever.com/zh/')">文档</span> |
          <span @click="$open('https://github.com/d2-projects/d2-admin-start-kit')">简化版</span> |
          <span @click="$open('https://alibaba.github.io/ice/scaffold?type=vue')">飞冰</span> |
          <span @click="$open('https://juejin.im/user/57a48b632e958a006691b946/posts')">掘金</span> |
          <span @click="$open('https://awesome.fairyever.com/daily/')">开发者日报</span> |
          <el-popover
            :width="172"
            trigger="hover">
            <p class="d2-mt-0 d2-mb-10">D2Projects</p>
            <img
              src="./image/qr@2x.png"
              style="width: 172px;">
            <span slot="reference">微信公众号</span>
            <p style="font-size: 12px; margin-top: 0px; margin-bottom: 0px;">
              官方公众号，主要推送前端技术类文章、框架资源、学习教程，以及 D2 系列项目更新信息
            </p>
          </el-popover>
        </div>
        <d2-badge/>
        <d2-help-btn/>
      </template>
    </d2-page-cover>
  </d2-container>
</template>

<script>
import D2HelpBtn from './components/d2-help-btn'
import D2Badge from './components/d2-badge'
export default {
  components: {
    D2HelpBtn,
    D2Badge
  },
  data () {
    return {
      filename: __filename
    }
  }
}
</script>

<style lang="scss" scoped>
.page {
  .page__logo {
    width: 120px;
  }
  .page__btn-group {
    color: $color-text-placehoder;
    font-size: 12px;
    margin-top: 0px;
    margin-bottom: 20px;
    span {
      color: $color-text-sub;
      &:hover {
        color: $color-text-main;
      }
    }
  }
}
</style>
