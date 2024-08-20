<template>
    <div>
        <h1>{{ props.title }}</h1>
        <slot></slot>
    </div>
</template>

<script setup>
const props = defineProps(['title'])

</script>

<style scoped>
div {
    border: 1px solid #ccc; /* 더 부드러운 회색으로 경계선 색상 변경 */
    border-radius: 8px; /* 둥근 모서리 추가 */
    max-width: 90vw; /* 최대 너비를 90%로 제한하여 양쪽에 여백 확보 */
    min-height: 10vh;
    margin: 0.5em auto; /* 상하 여백 추가 및 자동 중앙 정렬 */
    padding: 1em; /* 패딩을 좀 더 여유롭게 설정 */
    box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1); /* 부드러운 그림자 추가 */
    background-color: #f9f9f9; /* 약간의 배경색 추가 */
    box-sizing: border-box; /* 패딩과 경계선을 포함한 박스 크기 설정 */
}


</style>