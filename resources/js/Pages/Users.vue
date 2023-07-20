<script setup>
    import Layout from "./Shared/Layout.vue"
    import {Link} from "@inertiajs/vue3";
    import {defineProps} from "vue";

    const props = defineProps({
        time: String
    })

    defineOptions({ layout: Layout })
</script>

<template>
    <h1>Users</h1>
    <div style="margin-top: 1620px">
        <p class="text-blue-800">The time is {{ time }}</p>
        <Link href="/users" preserve-scroll>Refresh</Link>
    </div>
</template>
