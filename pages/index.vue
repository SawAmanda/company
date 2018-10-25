<template>
  <div class="container">
    <Header></Header>
    <Banner></Banner>
    <MainBusiness></MainBusiness>
  </div>
</template>

<script>
import Header from '../components/common/Header.vue' // 头部 logo nav
import Banner from '../components/Home/Banner.vue'; // 首页 Banner
import MainBusiness from '../components/Home/Mainbusiness.vue' // 首页 主营业务介绍
import Mainadvantage from '../components/Home/Mainadvantage.vue' // 首页 轻起来业务优势
import Techicalteam from '../components/Home/Techicalteam.vue' // 首页 专业的区块链+开发技术团队
import Platform from '../components/Home/Platform.vue' // 首页 全球创业者的加速孵化平台
import Media from '../components/Home/Media.vue' // 首页 合作媒体
import Power from '../components/Home/Power.vue' // 首页 为1300+企业服务的运维实力
import Footer from '../components/common/Footer.vue' // 页脚 footer


export default {
  components: {
    Header,
    Banner,
    MainBusiness,
    Mainadvantage,
    Techicalteam,
    Platform,
    Media,
    Power,
    Footer
  }
}
</script>

<style lang="scss">
@import '../assets/style.scss';
.container {
  width: 100%;
  position: relative;
  top: 0;
  left: 0;
}
</style>

