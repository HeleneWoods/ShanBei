<script setup>
defineProps({
  isTransform: {
    type: Boolean,
    default: false
  }
})
</script>

<template>
  <div class="banner-wrap" :class="{'transform-top': isTransform}">
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
}
.transform-top {
  transform: translate(-12px, -62px);
}
</style>