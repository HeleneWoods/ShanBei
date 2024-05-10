<script setup>
import mainItemBanner from '@/components/MainItemBanner.vue'
import mainItemBannerDesc from '@/components/MainItemBannerDesc.vue'
</script>

<template>
<div class="class-app">
  <mainItemBanner>
    <template #left>
      <mainItemBannerDesc>
        <template #desc-title-block>
          <div class="class-app-logo">
            <img class="content-block-info-title-en" width="282" height="25" src="https://media-image1.baydn.com/storage_media_image/kdbdns/a9efcc681a599e7648a8ee9223af5976.52154110a2ed4db66867bb22f403e3c4.png" alt="">
            <img class="content-block-info-title" width="42" src="https://media-image1.baydn.com/storage_media_image/kdbdns/569dfb4172a160b03a9f3597d39b24ab.f82b630c58fdf14e7a361dd3d39c5575.png">
            <span>扇贝课堂</span>
          </div>
        </template>
        <template #desc-detail-block>
          <div class="desc-detail-block">
            <p>
              一站式学习平台
            </p>
            <p>
              四六级、考研考试、职场技能、教资考证
            </p>
            <p>
              扇贝自主研发的精品课程
            </p>
          </div>
        </template>
        <template #desc-btn>
          <el-button class="desc-btn shanBei-download-btn">立即下载</el-button>
        </template>
      </mainItemBannerDesc>
    </template>
    <template #right>
      <img width="496" height="249" style="margin-top: 24px;" src="https://media-image1.baydn.com/storage_media_image/kdbdns/78cc5ff1b59f7832c78c4ca4a27c25be.1f8809dbefc7ec19e862d61f3387f053.png" alt="">
    </template>
  </mainItemBanner>
</div>
</template>

<style lang="scss" scoped>
.class-app {
  background-color: #f5f8fa;
}
.class-app-logo {
  display: flex;
  align-items: center;
  color: $themeColor;
  position: relative;

  span {
    margin-left: 16px;
    font-size: 32px;
  }
}
.content-block-info-title {
  z-index: 1;
}
.content-block-info-title-en {
  position: absolute;
  left: 0;
  top: -7px;
  z-index: 0;
}
.desc-detail-block {
  margin-top: 16px;
  font-size: 16px;
  line-height: 1.88;
  text-align: left;
}
.desc-btn {
  margin-top: 16px;
}
</style>