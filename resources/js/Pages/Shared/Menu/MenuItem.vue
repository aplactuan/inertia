<script setup>
    import {Link} from "@inertiajs/vue3";

    import {defineProps} from "vue";

    const props = defineProps({
        link: String,
        cmpnt: String
    })
</script>

<template>
    <li class="text-blue-800" :class="{'font-bold': $page.component == cmpnt}"><Link :href=link><slot /></Link></li>
</template>
