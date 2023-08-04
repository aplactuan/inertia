<script setup>
    import Layout from "./Shared/Layout.vue"
    import {Link, Head} from "@inertiajs/vue3";
    import {defineProps} from "vue";

    const props = defineProps({
        users: Array
    })

    defineOptions({ layout: Layout })
</script>

<template>
    <Head>
        <title>Users</title>
        <meta head-key="description" name="description" content="This is the users description" />

    </Head>
    <h1>Users</h1>
    <ul>
        <li v-for="user in users" key="user.id">{{ user.name }}</li>
    </ul>
</template>
