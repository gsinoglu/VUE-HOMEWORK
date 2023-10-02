<script setup>
const props = defineProps (['inputText', 'size'])
</script>



<template>
    <input type="" :class="{short}"> {{ props.inputText }}
</template>

<style scoped>
input{
    padding: 10px 40px;
    border-radius: 5px;
    background-color: white;
}
    .short{
        padding: 10px 20px; 
    }
    

</style>