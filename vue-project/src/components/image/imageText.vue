<script setup>
const props = defineProps(['text'])


</script>

<template>
    <p>{{ props.text }} </p>
</template>

<style scoped>

p {
    font-size: 18px;
    font-family:Arial, Helvetica, sans-serif;
    color: gray;
}
</style>