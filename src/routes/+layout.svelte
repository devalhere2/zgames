<script>
    import Header from "$lib/Header.svelte";
</script>

<Header/>
<slot />

<style>
    :root{
        --header-color: #272343;
        --body-color: #191A19;
    }
</style>
