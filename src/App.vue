<template>
  <router-view />
</template>
<script setup>
import { onMounted } from 'vue'
onMounted(() => {
  document.title = '马来西亚价值投资股票课程'
})
</script>
<style lang="less">
body {
  margin: 0;
  padding: 0;
}

h1,
h2,
h3,
h4,
h5,
h6,
ul,
p {
  margin: 0;
}

p {
  font-family: Helvetica;
}
</style>
