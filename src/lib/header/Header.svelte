<script lang="ts">
    import { page } from '$app/stores';
</script>

<header>

    <nav>
        <ul>
            <li class:active={$page.url.pathname === '/work'}>
                <a sveltekit:prefetch href="/work">Our Work</a>
            </li>
            <li class:active={$page.url.pathname === '/about'}>
                <a sveltekit:prefetch href="/about">About Us</a>
            </li>
            <li class:active={$page.url.pathname === '/contact'}>
                <a sveltekit:prefetch href="/contact">Contact Us</a>
            </li>
        </ul>
    </nav>

</header>