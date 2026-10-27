<svelte:head>
    <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:opsz,wght,FILL,GRAD@24,400,0,0&icon_names=keyboard_arrow_down" />
</svelte:head>

<script>
    export let titolo = "Titolo";
    export let elencoItem;
    export let isStatoMenuOpen = false;

    function mostraElenco(){
        isStatoMenuOpen = !isStatoMenuOpen
    }
</script>

<div id="header" on:click={mostraElenco}><p id="testo">{titolo}</p><span class="material-symbols-outlined">keyboard_arrow_down</span></div>

<style>
    #header {
        background-color: red;
        color: white;
        height: 50px;
        width: 300px;
        font-size: 1.5em;
        margin-top: 40px;
        border-radius: 15px;
    }

    #testo {
        width: 100%;
        height: 100%;
        display: flex;
        align-items: center;
        justify-content: center;
        font-size: 0.9em;
        font-weight: bold;
    }

    #header:hover {
        box-shadow: 0 0 0 4px rgb(255, 144, 144);
    }

    span {
        color: white;
    }
</style>