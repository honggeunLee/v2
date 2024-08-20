<template>
<MyVav></MyVav>
<div class="container">

    <MyTitle></MyTitle>

    <TodoContainer></TodoContainer>

</div>
</template>

<script setup>
import Counter1 from '../components/ex1/Counter1.vue';
import Counter2 from '../components/ex1/Counter2.vue';
import Ex1 from '../components/ex1/Ex1.vue';
import InputEx from '../components/ex2/InputEx.vue';
import MyContent from '../components/MyContent.vue';
import MyFooter from '../components/MyFooter.vue';
import MyTitle from '../components/MyTitle.vue';
import MyVav from '../components/MyVav.vue';

import SelectEx from '../components/ex2/SelectEx.vue';
import SelectEx2 from '../components/ex2/SelectEx2.vue';

import CountContainer from '../components/ex3/CountContainer.vue';
import TodoContainer from '../components/ex4/TodoContainer.vue';

const message = {sender: 'AAA', text: 'BBB'}

const mails = [
    {mno: 1, title: 'AAAA'},
    {mno: 2, title: 'BBBB'},
    {mno: 3, title: 'CCCC'},
    {mno: 4, title: 'DDDD'},
    {mno: 5, title: 'EEEE'}
]

const doA = () => {
    console.log('doA')
}

</script>

<style lang="scss" scoped>

</style>