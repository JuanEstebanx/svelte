<script>
    let someText = "More information send me Email.";
    let name = "JuanEstebanx GitHubProfile";
    let count = 0;
    let style = { darkMode: false };

    let webLogo =
        "https://w7.pngwing.com/pngs/161/231/png-transparent-war-dragons-dragon-city-dragon-war-game-dragon-army-game-dragon-video-game.png";
    let webLogoDark =
        "data:image/jpeg;base64,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";

    function handleClick() {
        count += 1;
    }

    function toggle() {
        style.darkMode = !style.darkMode;
        window.document.body.classList.toggle("dark-mode");
    }
</script>

<div class="About">
    <button on:click={handleClick}>
        Click Aquí {count == 0 ? "" : count}</button
    >
    <button on:click={toggle}>DarkMode</button>
    

    {#if !style.darkMode}
        <p>{someText}</p>
        <img src={webLogo} alt="Este es mi logo" />
    {:else}
        <p>
            <span>Hello DarkMode</span>
        </p>
        <img src={webLogoDark} alt="Este es mi logo" />
    {/if}
    <a href="https://github.com/JuanEstebanx">{name} </a>
</div>

<style>
    p {
        color: var (--theme-color);
    }
    p span {
        color: red;
    }
    img {
        width: 290px;
        height: 200px;
    }
</style>
