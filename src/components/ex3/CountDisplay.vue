<template>
    <div>
        <h1>COUNT DISPLAY</h1>
        <h1>{{ props.countObj.num }}</h1>
        <h1>{{ numValue }}</h1>
    </div>
</template>

<script setup>
import { computed } from 'vue';

const props = defineProps(['countObj'])

const numValue = computed(() => props.countObj.num)

</script>

<style lang="scss" scoped>

</style>