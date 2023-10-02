<script setup>
const props = defineProps(['button', 'color'])
const clickHandler = (event) => console.log('handler', eent)
</script>

<template>
    <button @click="clickHandler" :class="purple">{{ props.button }}</button>
</template>

<style scoped>
button {
    padding: 6px 90px;
    margin-top: 10px;
    background-color: white;
    font-size: 18px;
    color: black;
    border-radius: 5px;
}


.purple {
    padding: 6px 100px;
    margin-top: 10px;
    background-color: rgb(162, 0, 255);
    font-size: 18px;
    color: rgb(255, 255, 255);
    border-radius: 5px;
}
</style>