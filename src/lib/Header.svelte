<script>
    import { createEventDispatcher } from "svelte";
    const dispatch = createEventDispatcher();
    let toggle = false;
    function login() {
        toggle = !toggle;
        dispatch("loginToggle", toggle);
    }
</script>


<div id="header">
    <header>
        <div id="title">zGames</div>
        <button id="login" on:click={login}>Login</button>
    </header>    
</div>


<style>
    #header {
        width: 100vw;
        height: 80px;
        background-color: var(--body-color);
    }
    header {
        display: flex;
        justify-content: space-between;
        align-items: center;
        height: 80px;
        padding: 0px 10vw;
        background-color: var(--header-color);
        color: rgb(245, 222, 179);
        border-bottom: 1px solid rgba(245, 222, 179, 0.9);
        border-bottom-left-radius: 10px;
        border-bottom-right-radius: 10px;
        box-sizing: border-box;
    }
    #title {
        font-size: 30px;
        font-weight: bold;
    }

    #login {
        color: wheat;
        font-size: 20px;
        background-color: white;
        font-weight: bold;
        width: 100px;
        height: 40px;
        display: flex;
        justify-content: center;
        align-items: center;
        border-radius: 10px;
        background: linear-gradient(
            135deg,
            rgba(255, 255, 255, 0.1),
            rgba(255, 255, 255, 0)
        );
        backdrop-filter: blur(10px);
        -webkit-backdrop-filter: blur(10px);
        border: 1px solid rgba(245, 222, 179, 0.4);
        box-shadow: 0 8px 32px 0 rgba(0, 0, 0, 0.37);
        transition: all 250ms ease-in-out;
    }
    #login:hover {
        text-decoration: underline;
        background: transparent;
        border: none;
        font-size: 22px;
        cursor: pointer;
    }
</style>
