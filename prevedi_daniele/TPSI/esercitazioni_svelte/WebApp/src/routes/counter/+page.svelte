<script>
    import Counter from "#lib/components/counter.svelte";
    import DoubleCounter from "#lib/components/double_counter.svelte";

    let valoreSingolo = 127
    let valore = 0
</script>

<!--  chiamata di esempio con valore di partenza diverso da quello di default (definito nel componente) -->
<Counter bind:counter={valoreSingolo} />
<DoubleCounter bind:counter={valore}/>

<h3>Valore SingleCounter {valoreSingolo}</h3>
<h3>Valore DoubleCounter {valore}</h3>