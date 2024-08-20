<template>
    <div>
        <h1>Input Ex</h1>
        <div>
            <input type="text" v-model="input.v1">
        </div>
        <div>
            <input type="text" v-model="input.v2">
        </div>
        <h2>{{ input.v1 }}</h2>
        <h2>{{ input.v2 }}</h2>
    </div>
</template>

<script setup>
import { ref } from 'vue';

const input = ref({v1: 'AAA', v2: 'BBB'})

</script>

<style lang="scss" scoped>

</style>