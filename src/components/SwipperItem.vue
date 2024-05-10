<script setup>
defineProps({
  imgUrl: {
    type: String,
    required: true
  },
  // 默认往左滚动
  isLeft: {
    type: Boolean,
    default: true
  }
})

</script>

<template>
  <div class="img-wrapper">
    <div :class="isLeft ? 'left' : 'right'">
      <img :src="imgUrl" height="133" alt="">
      <img :src="imgUrl" height="133" alt="">
    </div>
  </div>
</template>

<style lang="scss" scoped>
@keyframes scrollLeft {
  0% {
    transform: translateX(0);
  }
  100% {
    transform: translateX(-50%);
  }
}
@keyframes scrollRight {
  0% {
    transform: translateX(-50%);
  }
  100% {
    transform: translateX(0);
  }
}
 
.img-wrapper {
  display: flex;
  height: 133px;
  white-space: nowrap;
}

.left {
  animation: scrollLeft 40s linear infinite;
}
.right {
  animation: scrollRight 40s linear infinite;
}
</style>