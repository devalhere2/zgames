<script>
    import Login from "$lib/Login.svelte";
    import { fade } from "svelte/transition";
</script>

<div id="body">
    <div in:fade={{ duration:250}} id="login">
        <Login />
    </div>
</div>

<style>
    :root {
        --header-color: #272343;
        --body-color: #191a19;
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
