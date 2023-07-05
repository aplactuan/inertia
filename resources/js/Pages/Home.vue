<script setup>
    import Layout from "./Shared/Layout.vue"

    defineProps({
        name: String,
        frameworks: Array
    })
</script>
<template>
    <Layout>
        <h1>Home</h1>
    </Layout>
</template>
