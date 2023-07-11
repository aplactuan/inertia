<script setup>
import {Link} from "@inertiajs/vue3";
import MenuItem from "./Menu/MenuItem.vue"
</script>

<template>
    <div>
        <ul class="flex space-x-4">
            <MenuItem link="/" cmpnt="Home">Home</MenuItem>
            <MenuItem link="/users" cmpnt="Users">Users</MenuItem>
            <MenuItem link="/settings" cmpnt="Settings">Settings</MenuItem>
            <li class="text-blue-800"><Link href="/logout-test" method="post" as="button" class="list-disc">Logout</Link></li>
        </ul>
    </div>

</template>
