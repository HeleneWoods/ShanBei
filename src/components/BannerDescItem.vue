<script setup>
defineProps({
  titleImg: {
    type: String
  },
  titleImgWidth: {
    type: String
  } 
})
</script>
<template>
  <div class="desc-wrap">
    <img :src="titleImg" :width="titleImgWidth" alt="">
    <p class="desc-details">
      <slot name="descDetails"></slot>
    </p>
    <el-button class="study-btn">开始学习</el-button>
  </div>
</template>

<style lang="scss" scoped>
.desc-details {
  color: rgba(255, 255, 255, 0.9);
}
.study-btn, .study-btn:hover {
  border-color: #fff;
  color: #fff;
  background-color: rgba(255, 255, 255, 0.2);
  margin-top: 16px;
}
</style>