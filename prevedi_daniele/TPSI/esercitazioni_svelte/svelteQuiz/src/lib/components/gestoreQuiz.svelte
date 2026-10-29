<script>
    import { numeroDomandeQuiz, avanzamentoQuiz } from "../js/store.js"

    export let domandeQuiz = []

    $numeroDomandeQuiz = domandeQuiz.children.length
    let punteggio = 0
</script>

<p>Domanda {avanzamentoQuiz} di {numeroDomandeQuiz} - Punteggio {punteggio}</p>
<progress max="{Number(numeroDomandeQuiz)}" value="{Number(avanzamentoQuiz)}"></progress>