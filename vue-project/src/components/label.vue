<script setup>
const props = defineProps(['text'])


</script>

<template>
    <label for="name">{{ props.text }} </label>
</template>

<style scoped>

label {
    font-size: 16px;
    font-family:Arial, Helvetica, sans-serif;
    color: rgb(89, 89, 89);
}

</style>