<script setup>
import theHeader from './components/TheHeader.vue'
import theBanner from './components/TheBanner.vue'
import wordsBanner from './views/WordsBanner.vue'
import readBanner from './views/ReadBanner.vue'
import listenBanner from './views/listenBanner.vue'
import programBanner from './views/ProgramBanner.vue'
import classBanner from './views/classBanner.vue'
import examBanner from './views/ExamBanner.vue'
import { ref } from 'vue'
const bannerData = ref([
  {
    imgLogo: 'https://media-image1.baydn.com/storage_media_image/bmpdqn/ace0086be8d3ace3601e90fccdc546c6.a2f9f948d6ecec0238721116c039f3aa.png',
    titleImg: 'https://media-image1.baydn.com/storage_media_image/bmpdqn/aa89e2a49749c378a7d400b053c42528.dce880554e63505910a7c24595159afb.png?x-oss-process=image/format,jpg/quality,q_80',
    titleImgWidth: '291',
    descDetails: ['独创专利真题例句关联学习法，智能关联当前词、已学词、待学词，反复记忆更牢固。', '发明专利号:CN113408275B']
  },
  {
    imgLogo: 'https://media-image1.baydn.com/storage_media_image/bmpdqn/b1713b5062ec9647070324916d72fedd.c6d54da46ea3256f5561aa351560916a.png',
    titleImg: 'https://media-image1.baydn.com/storage_media_image/bmpdqn/4efd4aabd5336d128ceaa20c38f22cbb.d3417f194379ea8de0e098b7c718951f.png?x-oss-process=image/format,jpg/quality,q_80',
    titleImgWidth: '291',
    descDetails: ['国内引入正版柯林斯高阶学习辞典，更有智慧词根、派生联想等扩展服务，按需选择。']
  },
  {
    imgLogo: 'https://media-image1.baydn.com/storage_media_image/bmpdqn/e4bdf035b821f7e3049be5e267368db8.76ee27537440884e287205cc94920627.png',
    titleImg: 'https://media-image1.baydn.com/storage_media_image/bmpdqn/92a782a391286e4815e4fd02e8242e62.2a806f88a605a877acc0a112767f430e.png?x-oss-process=image/format,jpg/quality,q_80',
    titleImgWidth: '351',
    descDetails: ['书库涵盖备考、职场、留学等词书，配套词典一词多义、熟词僻义。学无止境，未来可期。']
  }
])
</script>

<template>
  <div class="shanBei-layout">
    <div class="container">
      <div id="header">
        <theHeader />
      </div>
      <div id="main">
        <the-banner id="words" :bannerData="bannerData" />
        <words-banner />
        <read-banner id="read" />
        <listen-banner id="listen" />
        <program-banner id="program" />
        <class-banner />
        <exam-banner />
      </div>
      <div id="footer">footer</div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.shanBei-layout {
  width: 100vw;
}
#header {
  position: fixed;
  top: 0;
  width: 100%;
  z-index: 999;
}
#main {
  padding-top: 64px;
}
</style>
