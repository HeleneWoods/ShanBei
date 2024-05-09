<script setup>
defineProps({
  logoImg: {
    type: String
  }
})
</script>

<template>
  <div class="banner-item-wrap">
    <div class="banner-item-desc">
      <slot name="desc"></slot>
    </div>
    <img :src="logoImg" alt="banner-item-logo" class="banner-item-logo">
  </div>
</template>

<style lang="scss" scoped>
.banner-item-wrap {
  width: 940px;
  height: 100%;
  margin: 0 auto;
  display: flex;
}
.banner-item-desc {
  width: 290px;
  margin-top: 54px;
}
.banner-item-logo {
  margin-left: 189px;
  margin-top: 16px;
}
</style>