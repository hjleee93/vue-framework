<template>
  <main class="page">
    <h1>Join Page</h1>
    <form @submit.prevent="onSubmit">
      <p><input type="email" v-model="email" placeholder="email" /></p>
      <p><input type="password" v-model="password" placeholder="password" /></p>
      <p><input type="text" v-model="name" placeholder="name" /></p>
      <button type="submit"> submit </button>
    </form>
  </main>
</template>
<script setup lang="ts">
import { ref } from 'vue'


const email = ref('')
const password = ref('')
const name = ref('')


function onSubmit () {
  console.log('submit')
}

</script>
<style scoped lang="scss">
</style>