<script setup>
    import Nav from "./Nav.vue"
</script>
<template>
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
