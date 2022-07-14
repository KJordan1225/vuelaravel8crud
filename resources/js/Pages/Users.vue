<template>
     <h1 class="text-4xl font-bold">Users</h1>

    <div style="margin-top: 400px">
        The current time is {{ time }}
    </div>
    <Link href="/users" class="text-blue-500" preserve-scroll>Refresh</Link>
</template>

<script>    

    import  Layout  from '../Shared/Layout';
    import { Link } from '@inertiajs/inertia-vue3';

    export default {
        layout: Layout,

        props: {
            time: String
        }

    };
    
</script>








