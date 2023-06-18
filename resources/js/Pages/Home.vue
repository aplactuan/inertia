<script setup>
    defineProps({
        name: String,
        frameworks: Array
    })
</script>
<template>
    <h1>Hello {{ name}}</h1>
    <p>This is a website that uses the following</p>
    <ul>
        <li v-for="framework in frameworks">{{ framework }}</li>
    </ul>
</template>
