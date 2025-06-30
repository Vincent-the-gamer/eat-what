<script setup lang="ts" generic="T extends any, O extends any">
defineOptions({
  name: 'IndexPage',
})
</script>

<template>
  <div>
    <div i-hugeicons-serving-food inline-block text-4xl />
    <p>吃啥？</p>
    <p>
      <em text-sm op75>今天早上/中午/晚上到底吃啥？</em>
    </p>
    
    <div mt-4>
      <Raffle />
    </div>
  </div>
</template>


<style lang="css" scoped>

</style>