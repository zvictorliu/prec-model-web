<script setup>
import './assets/material-icons.scss' // 引入material-icons
import AppHeader from './components/AppHeader.vue'
import AppFooter from './components/AppFooter.vue'
</script>

<template>
  <div class="app-container">
    <AppHeader />
    <div class="app-content">
      <RouterView />
    </div>
    <AppFooter />
  </div>
</template>

<style scoped>
.app-container {
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  width: 100%;
  padding: 0;
}
.app-content {
  flex: 1;
  margin: 0 auto;
  padding-bottom: 60px; /* 给底部留空间 */
}
</style>
