<script setup>
import { RouterLink, RouterView } from 'vue-router'
import theHeader from './components/TheHeader.vue'
import welcome from './components/TheWelcome.vue'
</script>

<template>
  <div class="shanBei-layout">
    <div class="container">
      <div id="header">
        <theHeader />
      </div>
      <div id="main">
      </div>
      <div id="footer">footer</div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.shanBei-layout {
  width: 100vw;
}
#header {
  position: fixed;
  top: 0;
  width: 100%;
  z-index: 999;
}
#main {
  padding-top: 64px;
}
</style>
