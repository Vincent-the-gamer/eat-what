<template>
  <main font-sans p="x-4 y-10" text="center gray-700 dark:gray-200">

      <div i-hugeicons-serving-food inline-block text-4xl />
      <p>吃啥？</p>
      <p>
        <em text-sm op75>今天早上/中午/晚上到底吃啥？</em>
      </p>

      <Choose mt-2 />

      <div mt-2>
        <RouterView />
      </div>

    <Footer />
  </main>
</template>
