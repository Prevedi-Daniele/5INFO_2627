<script>
    import Domanda from "../components/domanda.svelte"
    import { numeroDomandeQuiz, avanzamentoQuiz } from "../js/store.js"

    export let domandeQuiz = []

    $numeroDomandeQuiz = domandeQuiz.length
    let punteggio = 0

</script>

<p>Domanda {$avanzamentoQuiz} di {$numeroDomandeQuiz} - Punteggio: {punteggio}</p>
<progress max="{Number($numeroDomandeQuiz)}" value="{Number($avanzamentoQuiz)}"></progress>

<Domanda domanda={domandeQuiz[$avanzamentoQuiz]} />