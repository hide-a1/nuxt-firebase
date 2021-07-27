<template>
  <div class="container">
      <button class="bg-blue-500 rounded text-white p-2" @click="login">
        ログイン
      </button>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  methods: {
    login() {
      console.log('login');
      this.$store.dispatch('login');
    }
  }
})
</script>

<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}
</style>
