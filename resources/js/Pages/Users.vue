<template>
    <h1 class="text-4xl font-bold">Users</h1>
    <Nav/>
    <div style="margin-top: 1024px">
        <p>The current time is {{ time }}.</p>
        <Link href="/users" class="text-blue-500 hover:underline" preserve-scroll>Refresh</Link>
    </div>
</template>
<script>
import Nav from "../Shared/Nav";
import {Link} from "@inertiajs/inertia-vue3";

export default {
    components: {Nav, Link},

    props: {time: String}
}
</script>
