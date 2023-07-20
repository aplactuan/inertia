<script setup>
    import Layout from "./Shared/Layout.vue"

    defineProps({
        name: String,
        frameworks: Array
    })

    defineOptions({ layout: Layout })
</script>
<template>
    <h1>Home</h1>
</template>
