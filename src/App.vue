<script setup lang="ts">
import { reactive } from "vue";

const data = reactive({
    count: 0,
});
</script>

<template>
    <ALayout class="root">
        <ALayoutHeader class="header">Header</ALayoutHeader>
        <ALayoutContent class="content">
            <ATypography>Count is: {{ data.count }}</ATypography>
            <AButton @click="() => data.count++">Click!</AButton>
        </ALayoutContent>
        <ALayoutFooter class="footer">Footer</ALayoutFooter>
    </ALayout>
</template>

<style lang="scss" scoped>
.root {
    .content {
        text-align: center;
    }
}
</style>
