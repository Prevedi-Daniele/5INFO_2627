<script>
    import { createEventDispatcher } from "svelte";
    const dispatch = createEventDispatcher()

    export let domanda

    let testoDomanda = domanda.domanda
    let arrayRisposte = Object.entries(domanda.risposte)

    console.log(arrayRisposte[0][1])

    // dispatch("rispostaSelezionata", {Boolean(rispostaGiusta) == true})
</script>

<h3>{testoDomanda}</h3>
<!-- {#each arrayRisposte as risposta}
    <button rispostaGiusta={risposta[1]} on:click={}>{risposta[0]}</button>
{/each} -->