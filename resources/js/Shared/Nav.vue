<template>
    <nav>
        <ul class="flex list-disc space-x-4 list-inside">
            <li><Link href="/" class="text-blue-500 hover:underline"
            :class="{'font-bold underline': $page.component == 'Home'}"
            >Home</Link></li>
            <li><Link href="/users" class="text-blue-500 hover:underline"
            :class="{'font-bold underline': $page.component == 'Users'}"
            >Users</Link></li>
            <li><Link href="/settings" class="text-blue-500 hover:underline"
            :class="{'font-bold underline': $page.component == 'Settings'}"
            >Settings</Link></li>
            <li>
                <Link href="/logout" method="post" as="button" class="text-blue-500 hover:underline">
                    Logout
                </Link>
            </li>
        </ul>
    </nav>
</template>

<script>   

    import { Link } from '@inertiajs/inertia-vue3';

    export default {
        components: { Link },

    };
</script>
