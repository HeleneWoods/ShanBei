<script setup>
import swipperItem from './SwipperItem.vue'
defineProps({
  scrollImgs: {
    type: Array,
    required: true
  },
  leftStart: {
    type: Boolean,
    default: true
  }
})

</script>

<template>
  <div class="swipper-window">
    <swipper-item
      v-for="(img, inx) in scrollImgs"
      :key="img"
      :imgUrl="img"
      :isLeft="leftStart ? inx % 2 === 0 : inx % 2 > 0" />
  </div>
</template>

<style lang="scss" scoped>
.swipper-window {
  height: 426px;
  width: 634px;
  overflow: hidden;
}
</style>