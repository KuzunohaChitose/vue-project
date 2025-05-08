<script setup lang="ts">
import { useCounterStore } from "@/stores/counter.ts";

const counterStore = useCounterStore();
</script>

<template>
    <ALayout class="root">
        <ALayoutHeader class="header">
            <h1>Count is: {{ counterStore.count }}</h1>
        </ALayoutHeader>
        <ALayoutContent class="content">
            <RouterView></RouterView>
        </ALayoutContent>
        <ALayoutFooter class="footer">Footer</ALayoutFooter>
    </ALayout>
</template>

<style lang="scss" scoped>
.root {
    width: 100%;
    height: 100%;

    .header {
        text-align: center;
        color: white;
    }

    .content {
        text-align: center;
    }

    .footer {
        text-align: center;
    }
}
</style>
