<script setup>
defineProps({
  btnTitle: {
    type: String
  },
  isTextRight: {
    type: Boolean,
    default: false
  }
})
</script>

<template>
  <div class="desc-wrap" :class="{'text-right': isTextRight}">
    <slot name="desc-title-block"></slot>
    <slot name="desc-detail-block"></slot>
    <slot name="desc-btn"></slot>
  </div>
</template>

<style lang="scss" scoped>
.desc-wrap {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  justify-content: flex-end;
  margin-bottom: 100px;
}
.text-right {
  align-items: flex-end;
}
</style>