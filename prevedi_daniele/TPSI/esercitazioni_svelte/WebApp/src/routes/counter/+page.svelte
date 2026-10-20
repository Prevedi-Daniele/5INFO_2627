<script>
    import Counter from "#lib/components/counter.svelte";
    import DoubleCounter from "#lib/components/double_counter.svelte";

    let valoreSingolo = 127
    let valoreDoppio = 0
</script>

<!--  chiamata di esempio con valore di partenza diverso da quello di default (definito nel componente) -->
<Counter bind:counter={valoreSingolo} />
<DoubleCounter bind:counter={valoreDoppio}/>

<h3>Valore SingleCounter {valoreSingolo}</h3>

{#if valoreDoppio < 5}
    <h3 class="rosso">Valore DoubleCounter {valoreDoppio}</h3>
{:else}
    <h3 class="verde">Valore DoubleCounter {valoreDoppio}</h3>
{/if}


<style>
    .rosso{color: red;}
    .verde{color: green;}
</style>