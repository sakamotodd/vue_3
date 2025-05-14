<script setup lang="ts">
import { ref } from 'vue'

const title = 'test'
const num = ref(1)

console.log(num.value)

function plus() {
  num.value += 1
}
</script>

<template>
  <h1>hoge {{ title }}</h1>
  <h1>hoge ${{ num }}</h1>
  <button @click="plus">ボタン</button>
</template>
