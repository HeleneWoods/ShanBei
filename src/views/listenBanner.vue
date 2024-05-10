<script setup>
import mainItemBanner from '@/components/MainItemBanner.vue'
import mainItemBannerDesc from '@/components/MainItemBannerDesc.vue'
import theSwipper from '@/components/TheSwipper.vue'

import { ref } from 'vue'

const scrollImgs = ref([
  'https://media-image1.baydn.com/storage_media_image/bmpdqn/7827cb7051a45ee0dfc6acda63a3a3b7.d019c34b0ed3f3a958c2451d81b375d3.png',
  'https://media-image1.baydn.com/storage_media_image/reweoz/5521aad5667fb71c9a4bc648936d500d.eeb65a1834575f0b2444857a825c7128.png',
  'https://media-image1.baydn.com/storage_media_image/bmpdqn/a54b0a7337af0b5db951761c4e84670c.1dae14d6a4703073eb88c23071f89bb5.png'
])
</script>

<template>
<div class="listen-app">
  <mainItemBanner height="564px">
    <template #left>
      <the-swipper :scrollImgs="scrollImgs" :leftStart="false" />
    </template>
    <template #right>
      <mainItemBannerDesc>
        <template #desc-title-block>
          <div class="listen-app-logo">
            <img class="content-block-info-title-en" width="240" height="24" src="https://media-image1.baydn.com/storage_media_image/bmpdqn/d918f4f201a26993618efa1e5a530407.39df4757bf60de3a48644877484966b5.png" alt="">
            <img class="content-block-info-title" width="42" src="https://media-image1.baydn.com/storage_media_image/bmpdqn/8e21001064cb3a247cdfd29f16b19998.8b5613e86d7f181c5a90b93f7687bd5a.png">
            <span>扇贝听力口语</span>
          </div>
        </template>
        <template #desc-detail-block>
          <div class="desc-detail-block">
            <p>
              12w+精选英文素材畅学
            </p>
            <p>
              中英字幕随机切换泛听
            </p>
            <p>
              6大精听/口语模式，逐句提高
            </p>
            <p>
              听力口语学习计划随心选
            </p>
          </div>
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
.listen-app {
  background-color: #f5f8fa;
}
.listen-app-logo {
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