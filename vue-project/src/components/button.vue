<script setup>
const props = defineProps(['button', 'color']);
const emits = defineEmits(['handler']);

const clickHandler = (event) => {
    if (props.color) {emits ('handler', props.color)}
    else { emits('handler', 'red');}
};
</script>

<template>
    <button @click="clickHandler" :class="props.color">{{ props.button }}</button>
</template>

<style scoped>
button {
    padding: 6px 90px;
    margin-top: 10px;
    background-color: white;
    font-size: 18px;
    color: black;
    border-radius: 12px;
}


.purple {
    background-color:blueviolet; 
    color: white;
    border-color: blueviolet;
}
</style>