<script setup>
import mainItemBanner from '@/components/MainItemBanner.vue'
import mainItemBannerDesc from '@/components/MainItemBannerDesc.vue'
import theSwipper from '@/components/TheSwipper.vue'

import { ref } from 'vue'

const scrollImgs = ref([
  'https://media-image1.baydn.com/storage_media_image/bmpdqn/90b8ad84ce9ae5b59e663d0e551c3ebe.907a594802c66a5080602267f3ca8e1f.png',
  'https://media-image1.baydn.com/storage_media_image/bmpdqn/dbaff60d4bde383dbf2998ab3ee7dd72.312812d5d87f93ce30dd2e313626a550.png',
  'https://media-image1.baydn.com/storage_media_image/bmpdqn/4d4cb3309ac9f26a112bfccbc7de7dae.c21b8a63e7a625ad0205cefa1b042f4b.png'
])
</script>

<template>
<div class="read-app">
  <mainItemBanner height="564px">
    <template #left>
      <mainItemBannerDesc>
        <template #desc-title-block>
          <div class="read-app-logo">
            <img class="content-block-info-title-en" width="239" height="24" src="https://media-image1.baydn.com/storage_media_image/bmpdqn/48a59bd6d72f5f4bf1a50e1d3e4c5a62.e2556b8f0c6a6fd759cd6ab1863e72bc.png" alt="">
            <img class="content-block-info-title" width="42" src="https://media-image1.baydn.com/storage_media_image/bmpdqn/a63e7ac093a94feaa05fbc16b9a51665.b6f2147b072d059238aedcacef3b0627.png">
            <span>扇贝阅读</span>
          </div>
        </template>
        <template #desc-detail-block>
          <div class="desc-detail-block">
            <p>
              海量英文原版
            </p>
            <p>
              大纲词汇、地道短语自动标注
            </p>
            <p>
              生词即点即查，读完立即进行巩固
            </p>
            <p>
              主题阅读计划随心选
            </p>
          </div>
        </template>
        <template #desc-btn>
          <el-button class="desc-btn shanBei-download-btn">立即下载</el-button>
        </template>
        <template #desc-extra-block>
          <img class="desc-extra-block" width="240" height="66" src="https://media-image1.baydn.com/storage_media_image/bmpdqn/e038a486465a553e869e3b0913d3089b.a89526bbe7f4297b611764c1b7000f2d.png" alt="">
        </template>
      </mainItemBannerDesc>
    </template>
    <template #right>
      <the-swipper :scrollImgs="scrollImgs" />
    </template>
  </mainItemBanner>
</div>
</template>

<style lang="scss" scoped>
.read-app-logo {
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
.desc-extra-block {
  margin-top: 32px;
}
</style>