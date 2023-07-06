<script setup>
    import Nav from "./Nav.vue"
</script>
<template>
    <header>
        <div class="max-w-7xl mx-auto">
            <div class="flex justify-between">
                <h1>App Name</h1>
                <Nav />
            </div>
        </div>
    </header>

    <slot />
</template>
