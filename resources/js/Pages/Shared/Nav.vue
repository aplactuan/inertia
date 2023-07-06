<script setup>
import {Link} from "@inertiajs/vue3";
</script>

<template>
    <div>
        <ul class="flex space-x-4">
            <li class="text-blue-800" :class="{'font-bold': $page.component == 'Home'}"><Link href="/">Home</Link></li>
            <li class="text-blue-800" :class="{'font-bold': $page.component == 'Users'}"><Link href="/users">Users</Link></li>
            <li class="text-blue-800" :class="{'font-bold': $page.component == 'Settings'}"><Link href="/settings">Settings</Link></li>
            <li class="text-blue-800"><Link href="/logout-test" method="post" as="button" class="list-disc">Logout</Link></li>
        </ul>
    </div>

</template>
