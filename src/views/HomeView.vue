<script setup lang="ts">
import { useCounterStore } from "@/stores/counter.ts";

const counterStore = useCounterStore();
</script>

<template>
    <div class="home">
        <div>
            <h1>This is a home page</h1>
            <RouterLink to="/about">About Page</RouterLink>
            <ADivider></ADivider>
            <AButton @click="counterStore.increment" type="primary">Increment</AButton>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.home {
    min-height: 80vh;
    display: flex;
    align-items: center;
    justify-content: center;
}
</style>
