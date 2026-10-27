<script>
    import Dropdown from "#lib/components/dropdown.svelte";
</script>

<h1>DROP DOWN TESTER</h1>

<Dropdown titolo="Regione" elencoItem={["Piemonte", "Lombardia", "Lazio", "Liguria", "Puglia"]} isStatoMenuOpen={false}/>
<Dropdown titolo="Città" elencoItem={["Torino", "Milano", "Roma", "Genova"]} isStatoMenuOpen={false}/>
<Dropdown titolo="Nazione" elencoItem={["Italia", "Francia", "Germania", "Olanda"]} isStatoMenuOpen={false}/>