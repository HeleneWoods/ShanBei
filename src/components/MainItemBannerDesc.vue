<script setup>
defineProps({
  width: {
    type: String
  },
  isTextRight: {
    type: Boolean,
    default: false
  }
})
</script>

<template>
  <div class="desc-wrap" :style="{'width': width}" :class="{'text-right': isTextRight}">
    <slot name="desc-title-block"></slot>
    <slot name="desc-detail-block"></slot>
    <slot name="desc-btn"></slot>
    <slot name="desc-extra-block"></slot>
  </div>
</template>

<style lang="scss" scoped>
.desc-wrap {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  justify-content: flex-end;
}
.text-right {
  align-items: flex-end;
}
</style>