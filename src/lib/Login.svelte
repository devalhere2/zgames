<form id="card">
    <div id="title">
        <h1>Login</h1>
    </div>
    <div class="usp">
        <label for="username">Username:</label>
        <input type="text" id="username" name="username" required />
    </div>
    <div class="usp">
        <label for="password">Password:</label>
        <input type="password" id="password" name="password" required />
    </div>
    <div id="rme">
        <input type="checkbox" id="rme-checkbox" name="rme" />
        <label for="rme-checkbox">Remember me</label>
    </div>
    <div id="buttons">
        <button id="login" type="submit">Login</button>
        <button id= "create" type="button">Create Account</button>
    </div>
</form>

<style>
    #card {
        display: flex;
        align-items: center;
        flex-direction: column;
        font-weight: bold;
        height: 54vh;
        width: 24vw;
        border-radius: 10px;
        background: linear-gradient(
            135deg,
            rgba(255, 255, 255, 0.1),
            rgba(255, 255, 255, 0)
        );
        backdrop-filter: blur(10px);
        -webkit-backdrop-filter: blur(10px);
        border: 1px solid rgba(255, 255, 255, 0.18);
        box-shadow: 0 8px 32px 0 rgba(47, 47, 47, 0.245);
    }
    #title {
        height: 20%;
        width: 100%;
        display: flex;
        justify-content: center;
        align-items: center;
        text-decoration: underline;
        transform: translateY(5px);
        /* background-color: red; */
    }
    .usp {
        display: flex;
        flex-direction: column;
        align-items: center;
        width: 100%;
        height: 20%;
    }
    .usp input {
        height: 40px;
        width: 88%;
        border-radius: 10px;
        border-width: 0px;
        background-color: transparent;
        border: 1px solid rgba(255, 255, 255, 0.37);
        color: rgb(189, 189, 255);
        font-weight: bold;
        font-family: 'Courier New', Courier, monospace;
        font-size: 20px;
        padding-left: 10px;
    }
    .usp label {
        font-size: 20px;
        display: flex;
        padding: 5px;
        width: 90%;
        background-color: transparent;

    }

    #rme {
        display: flex;
        align-items: flex-end;
        width: 88%;
    }
    #rme input[type="checkbox"] {
        margin-right: 10px;
    }

    #rme label {
        margin: 0;
    }

    #buttons {
        display: flex;
        justify-content: space-around;
        flex-direction: column;
        width: 60%;
        height: 32%;
        padding-top: 5px;
    }

    #login {
        height: 50px;
        border-radius: 10px;
        border: 1px solid rgba(255, 255, 255, 0.37);
        background-color: wheat;
        font-size: 20px;
        font-weight: bold;
        font-family: 'Courier New', Courier, monospace;        
}
    #create {
        height: 50px;
        border-radius: 10px;
        border: 1px solid rgba(255, 255, 255, 0.37);
        background-color: transparent;
        font-size: 20px;
        color: wheat;
        font-weight: bold;
        font-family: 'Courier New', Courier, monospace;
    }
</style>
