<script setup>
    import Nav from "./Shared/Nav.vue"
    import {Link} from "@inertiajs/vue3";
    import {defineProps} from "vue";

    const props = defineProps({
        time: String
    })
</script>

<template>
  <h1>Users</h1>
  <Nav />
  <div style="margin-top: 1620px">
      <p class="text-blue-800">The time is {{ time }}</p>
      <Link href="/users" preserve-scroll>Refresh</Link>
  </div>
</template>
