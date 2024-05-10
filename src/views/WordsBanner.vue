<script setup>
import mainItemBanner from '@/components/MainItemBanner.vue'
import mainItemBannerDesc from '@/components/MainItemBannerDesc.vue'
</script>

<template>
<div class="words-app">
  <mainItemBanner :isTransform="true">
    <template #left>
      <div class="swiper-wrap">
        <div class="swiper-item"></div>
      </div>
    </template>
    <template #right>
      <mainItemBannerDesc class="desc-wrap" :isTextRight="true">
        <template #desc-title-block>
          <div class="words-app-logo">
            <img width="32" src="https://media-image1.baydn.com/storage_media_image/bmpdqn/e03c60afe9723757ad81c10edeb3caa9.e14c2536f243eb8236b474b152e97d09.png">
            <span>扇贝单词</span>
            <span>英语版</span>
          </div>
        </template>
        <template #desc-detail-block>
          <p class="desc-detail-block">
            和亿万用户一起背单词
          </p>
        </template>
        <template #desc-btn>
          <el-button class="desc-btn shanBei-download-btn">立即下载</el-button>
        </template>
      </mainItemBannerDesc>
    </template>
  </mainItemBanner>
</div>
</template>

<style lang="scss" scoped>
.words-app {
  background-color: #f5f8fa;
  height: 340px;
}
.swiper-wrap {
  height: 390px;
  width: 620px;
}
.words-app-logo {
  display: flex;
  align-items: center;
  color: $themeColor;

  span:first-of-type {
    margin-left: 16px;
    font-size: 32px;
    font-weight: 500;
  }
  span:last-of-type {
    margin-left: 4px;
    font-size: 16px;
  }
}
.desc-detail-block {
  margin-top: 4px;
  font-size: 16px;
  font-weight: bold;
}
.desc-btn {
  margin-top: 37px;
}
</style>