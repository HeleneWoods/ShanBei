<script setup>
defineProps({
  height: {
    type: String,
    default: '420px'
  },
  isTransform: {
    type: Boolean,
    default: false
  }
})
</script>

<template>
  <div class="banner-wrap" :style="{'height': height}" :class="{'transform-top': isTransform}">
    <slot name="left"></slot>
    <slot name="right"></slot>
  </div>
</template>

<style lang="scss" scoped>
.banner-wrap {
  display: flex;
  justify-content: space-between;
  text-align: center;
  width: 940px;
  margin: 0 auto;
  align-items: center;
}
.transform-top {
  transform: translate(-12px, -62px);
}
</style>