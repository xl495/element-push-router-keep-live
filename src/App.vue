<script setup lang="ts">
</script>

<template>
  <el-button type="primary" @click="$router.push('/')" >TABLE Page</el-button>
  <el-button type="success" @click="$router.push('/home')" >Home Page</el-button>
  <router-view  v-slot="{ Component }">
      <keep-alive :include="['Table']" >
          <component :is="Component" />
        </keep-alive>
    </router-view>
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
