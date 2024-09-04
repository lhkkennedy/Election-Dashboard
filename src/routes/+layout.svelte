<script>
    import "tailwindcss/tailwind.css";
    import NavBar from "../lib/components/navBar.svelte";
    import { page } from '$app/stores';  
    let currentPath = $page.url.pathname
</script>

{#if currentPath = ""}
<NavBar />
{/if}

<slot />