<script setup lang="ts" generic="T extends any, O extends any">
defineOptions({
  name: 'IndexPage',
})

const foods = ref<string[]>([])
</script>

<template>
  <div>
    <div i-hugeicons-serving-food inline-block text-4xl />
    <p>吃啥？</p>
    <p>
      <em text-sm op75>今天早上/中午/晚上到底吃啥？</em>
    </p>
    
    <div mt-4>
      <p>输入你想吃的食物，一行一个: </p>
      <textarea v-model="foods" />
    </div>

  </div>
</template>


<style lang="css" scoped>
textarea {
  width: 20rem;
  height: 8rem;
  border: 1.2px solid deeppink;
  border-radius: 4px;
}
</style>