<script setup>
import bannerItem from './BannerItem.vue'
import bannerDescItem from './BannerDescItem.vue'
defineProps({
  bannerData: {
    type: Array,
    required: true
  }
})
</script>

<template>
  <div class="banner-wrap">
    <el-carousel height="320px" arrow="never" :pause-on-hover="false" >
      <el-carousel-item v-for="item in bannerData" :key="item">
        <bannerItem :logoImg="item.imgLogo">
          <template #desc>
            <banner-desc-item :titleImg="item.titleImg" :titleImgWidth="item.titleImgWidth">
              <template #descDetails>
                <p v-for="info in item.descDetails" :key="info" class="desc-details">{{info}}</p>
              </template>
            </banner-desc-item>
          </template>
        </bannerItem>
      </el-carousel-item>
    </el-carousel>
  </div>
</template>

<style lang="scss" scoped>
.banner-wrap {
  height: 320px;
  background-color: $themeColor;
}
.desc-details:not(:first-child) {
  margin-top: 12px;
}
// 改变指示器样式
:deep(.el-carousel__indicators--horizontal) {
  bottom: 76px;
}
:deep(.el-carousel__button) {
  width: 8px;
  height: 8px;
  border-radius: 50%;
}
</style>