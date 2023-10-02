<script setup>
const props = defineProps(['head'])


</script>

<template>
    <h2>{{ props.head }}</h2>
</template>

<style scoped>

h2 {
    font-size: 24px;
    font-family:Arial, Helvetica, sans-serif;
    color: black;
    margin: 10px 0px 0px;
}

</style>