<template>
    <div class="row g-3">
        <div class="col-md-6 col-lg-4 col-xl-3" v-for="{pno, pname, price, sale} in saleProducts" :key="pno" v-show="sale">
            <h2>{{ pname }}</h2>
            <p>{{ price }}HTML is the standard markup language for describing the structure of the web pages. Our HTML tutorials will help you to understand the basics of latest HTML5 language, so that you can create your own website.</p>
            <p><a href="https://www.tutorialrepublic.com/html-tutorial/" target="_blank" class="btn btn-success">Learn More &raquo;</a></p>
        </div>
    </div>
</template>

<script setup>
import { computed, reactive } from 'vue';

const props = defineProps(["src"])
console.log(props.src);


const arr = reactive([
    {pno: 1, pname: 'p1', price: 3000, sale: true},
    {pno: 2, pname: 'p2', price: 4000, sale: false},
    {pno: 3, pname: 'p3', price: 5000, sale: true},
    {pno: 4, pname: 'p4', price: 6000, sale: false}
])

const saleProducts = computed(() => arr.filter(item => item.sale));

setTimeout(() => {
    arr.push({pno: 5, pname: 'p5', price: 6000, sale: true})
    arr.push({pno: 6, pname: 'p6', price: 6000, sale: true})
}, 3000)

</script>

<style lang="scss" scoped>

</style>