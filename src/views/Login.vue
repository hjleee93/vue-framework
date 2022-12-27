<template>
  <main class="page">
    <h1>Login Page</h1>
    <form @submit.prevent="onSubmit">
      <p><input type="email" v-model="email" placeholder="email" /></p>
      <p><input type="password" v-model="password" placeholder="password" /></p>
      <button type="submit"> login</button>
      <button @click="$router.push('/join')">Join</button>

    </form>
  </main>
</template>
<script setup lang="ts">
import { ref } from 'vue'

const email = ref('')
const password = ref('')


function onSubmit () {
  console.log('submit')
}

</script>
<style scoped lang="scss">
</style>