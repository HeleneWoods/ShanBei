<script setup>
import mainItemBanner from '@/components/MainItemBanner.vue'
import mainItemBannerDesc from '@/components/MainItemBannerDesc.vue'
</script>

<template>
<div class="exam-app">
  <mainItemBanner>
    <template #left>
      <img width="686" height="344" src="https://media-image1.baydn.com/storage_media_image/konioc/f9bc8c8053e86c3916f7087cdf18b399.d713429f00893a245d8aae335a995d92.png" alt="">
    </template>
    <template #right>
      <mainItemBannerDesc>
        <template #desc-title-block>
          <div class="exam-app-logo">
            <img width="32" src="https://media-image1.baydn.com/storage_media_image/konioc/9c44cec487edecd002bc3dc2f7c44493.159cf4ecbd113b719558970368604d7b.png">
            <span>扇贝考研</span>
          </div>
        </template>
        <template #desc-detail-block>
          <div class="desc-detail-block">
            <p>
              考研学习平台
            </p>
            <p>
              真题，单词，课程，一站式学习
            </p>
          </div>
        </template>
        <template #desc-btn>
          <div class="btn-group">
            <el-button class="desc-btn shanBei-download-btn">IOS下载</el-button>
            <el-button class="desc-btn shanBei-download-btn">安卓下载</el-button>
          </div>
        </template>
      </mainItemBannerDesc>
    </template>
  </mainItemBanner>
</div>
</template>

<style lang="scss" scoped>
.swiper-wrap {
  height: 390px;
  width: 620px;
}
.exam-app-logo {
  display: flex;
  align-items: center;
  color: $themeColor;

  span {
    margin-left: 16px;
    font-size: 32px;
  }
}
.desc-detail-block {
  margin-top: 16px;
  font-size: 16px;
  line-height: 1.88;
  text-align: left;
}
.btn-group {
  display: flex;
  margin-top: 16px;
}
</style>