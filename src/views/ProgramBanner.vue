<script setup>
import mainItemBanner from '@/components/MainItemBanner.vue'
import mainItemBannerDesc from '@/components/MainItemBannerDesc.vue'
</script>

<template>
<div class="program-app">
  <mainItemBanner>
    <template #left>
      <img width="544" height="300" src="https://media-image1.baydn.com/storage_media_image/dndrgt/dc774755526690f70523b672e8a8a81f.1fd4bfdbbefd482b421d5269f4fe508c.png" alt="">
    </template>
    <template #right>
      <mainItemBannerDesc width="280px">
        <template #desc-title-block>
          <div class="program-app-logo">
            <img class="content-block-info-title-en" width="199" height="24" src="https://media-image1.baydn.com/storage_media_image/bmpdqn/009794a719d6c7456ea6f2ffef952a22.a9c99b8c87953166a5e42fb302cccfb4.png" alt="">
            <img class="content-block-info-title" width="32" src="https://media-image1.baydn.com/storage_media_image/dndrgt/0db318f7b3b6ca141f805c43f7c406a8.502a08aaeacc0f53b36c2240ef0cf033.png">
            <span>扇贝编程</span>
          </div>
        </template>
        <template #desc-detail-block>
          <div class="desc-detail-block">
            <p>
              互动新课堂
            </p>
            <p>
              理论+实战，在线写代码
            </p>
            <p>不用下载软件</p>
            <p>助教老师答疑</p>
          </div>
        </template>
        <template #desc-btn>
            <el-button class="desc-btn shanBei-download-btn">立即报名</el-button>
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
.program-app-logo {
  display: flex;
  align-items: center;
  color: #1029a3;
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