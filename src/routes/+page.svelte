<script>
    import Header from "$lib/Header.svelte";
    import Login from "$lib/Login.svelte";
    import { fade } from "svelte/transition";
    let loginTogglestate;
    function loginToggle(event) {
        loginTogglestate = event.detail;
    }
</script>

<Header on:loginToggle={loginToggle} />

<div id="body">
    {#if loginTogglestate}
        <div transition:fade id="login">
            <Login />
        </div>
    {/if}
</div>

<style>
    :root{
        --header-color: #272343;
        --body-color: #191A19;
    }
    #body {
        display: flex;
        justify-content: center;
        align-items: center;
        height: calc(100vh - 80px);
        background-color: var(--body-color);
        color: rgb(245, 222, 179);
        width: 100vw;
    }
</style>
