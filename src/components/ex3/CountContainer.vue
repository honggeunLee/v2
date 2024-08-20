<template>
    <div>
        <h1>COUNT CONTAINER</h1>
        <CountDisplay :countObj="countObj"></CountDisplay>
        <hr>
        <CountButtons @changeCount="changeCount"></CountButtons>
    </div>
</template>

<script setup>
import { ref } from 'vue';
import CountButtons from './CountButtons.vue';
import CountDisplay from './CountDisplay.vue';

const countObj = ref({num: 10})

const changeCount = (amount) => {
    countObj.value.num += amount
}

</script>

<style lang="scss" scoped>

</style>