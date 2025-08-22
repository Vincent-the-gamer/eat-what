<template>
    <div flex="~ justify-center items-center gap-2">
        <span @click="$router.push('/')" :class="{ active: routerPath === '/' }">随机抽取</span>
        <span @click="$router.push('/order')" :class="{ active: routerPath === '/order' }">有序规划</span>
    </div>

</template>

<script setup lang="ts">
const router = useRouter()

const routerPath = ref<string>(router.currentRoute.value.path)

watch(() => router.currentRoute.value, (newVal) => {
    routerPath.value = newVal.path
})
</script>

<style scoped>
span {
    cursor: pointer;
    background-color: aquamarine;
    border-radius: 6px;
    padding: 4px 8px;
    border: 1.5px solid yellowgreen;

    &:hover {
        background-color: black;
        color: white;
    }

    &.active {
        background-color: orange;
        color: white;
    }
}
</style>