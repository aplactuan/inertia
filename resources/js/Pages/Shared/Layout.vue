<script setup>
    import Nav from "./Nav.vue"
    import { Head } from "@inertiajs/vue3";
</script>
<template>
    <Head>
        <title>My App</title>
        <meta name="description" content="Global Description" head-key-="description">
    </Head>
    <header>
        <div class="max-w-7xl mx-auto">
            <div class="flex justify-between">
                <div class="flex items-center">
                    <h1>App Name</h1>
                    <p class="ml-4">
                        Welcome {{ $page.props.auth.username }}
                    </p>
                </div>
                <Nav />
            </div>
        </div>
    </header>

    <slot />
</template>
