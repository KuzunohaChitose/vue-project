<script setup lang="ts">
import { useCounterStore } from "@/stores/counter.ts";

const counterStore = useCounterStore();
</script>

<template>
    <div class="about">
        <div>
            <h1>This is an about page</h1>
            <RouterLink to="/">Home Page</RouterLink>
            <ADivider></ADivider>
            <AButton @click="counterStore.increment" type="primary">Increment</AButton>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.about {
    min-height: 80vh;
    display: flex;
    align-items: center;
    justify-content: center;
}
</style>
