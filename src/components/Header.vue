<template>
  <ul>
    <li @click="$router.push('/')"><img alt="Vue logo" class="logo" src="@/assets/logo.svg" width="50" height="50" />Home</li>
    <li @click="$router.push('/about')">About</li>
    <li @click="$router.push('/login')">Login</li>
    
  </ul>
</template>
<script setup lang="ts">
</script>
<style scoped lang="scss">
ul{
  list-style: none;
  display: flex;
  height: 80px;
  justify-items: center;
  align-items: center;
  background-color: #fff;
  color: #000;
  li{
    cursor: pointer;
    margin-right: 10px;
    display: flex;
    align-items: center;

  }
}
</style>