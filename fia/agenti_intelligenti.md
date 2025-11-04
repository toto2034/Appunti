## Agenti Intelligenti

Agente è un qualsiasi cosa possa essere vista come un sistema che percepisce il suo ambiente attraverso sensori ed agisce su di esse tramite degli attuatori

Ad esempio: Un umano è un agente perchè utilizza come sensori (i sensi), occhi, orecchie naso e utilizza degli attuatori

Definizione di Percezione:  Insieme di input percettivi dell’agente in un dato istante.
Definizione di Sequenza percettiva: la storia completa di tutto ciò che l'agente ha percepito nella sua esistenza

Un'azione dell'agente, in un qualsiasi istante, può dipendere dall'intera sequenza, ma non daqualcosa che non abbia percepito.

### Cosa rende un agente intelligente o stupido?

Prestazione, Conoscenza pregressa, Azioni che l'agente può compiere, Sequenza percettiva fino all'istante corrente

La **razionalità** di un agente, dipende da questi quattro fattori, questo è razionale in base alle sue conoscenze, al suo obiettivo, oltre che al contesto che lo circonda.

Quindi un agente razionale dovrebbe scegliere un'azione che massimizzi il valore atteso della sua **misura di prestazione**. 

La **misura di prestazione** dovrebbe essere progettata sulla base dell’effetto che si desidera osservare sull’ambiente e non su come dovrebbe comportarsi l’agente. Altrimenti, un agente otterrebbe una razionalità perfetta semplicemente “illudendosi” di fare la cosa giusta.

La razionalità non implica l'onniscienza. Un agente onnisciente conosce il risultato effettivo delle sue azioni e può agire di conseguenza (impossibile), mentre un agente razionale fa la cosa giusta sulla base del contesto in cui opera. Razionalità non significa perfezione ma **massimizzione del risultato atteso**.

**Information gathering**, sono delle azioni che hanno la sola finalità di raccogliere informazioni sull'ambiente circostante e che consentono di modificare le percezioni future per massimizzare il risultato atteso. 
*es. l’azione di guardare a destra e sinistra prima di attraversare la strada. Oppure * **l'esplorazione** * per far conoscenza su un ambiente sconosciuto*. L'esplorazione prevede il concetto di apprendimento, la capacità di imparare coppie di percezioni-azioni. Infatti non possiamo chiamare un agente autonomo se intraprende azioni inserite nella sua fase di progettazione e non dalle sue percezioni.

### Ambiente

Un **ambiente** viene generalmente descritto tramile la formulazione PEAS:
- **P.** Misura di *prestazione* adottata per valutare l’operato di un agente.
- **E.** Descrizione degli *elementi* che formano l’ambiente.
- **A.** Gli *attuatori* disponibili all’agente per intraprendere le azioni.
- **S.** I *sensori* attraverso i quali riceve gli input percettivi.

Se la **varietà di ambienti** operativi nell’intelligenza artificiale è molto vasto, possiamo identificare un numero relativamente piccolo di dimensioni per caratterizzarli:

- Completamente o parzialmente **osservabili**. I sensori di un ambiente danno accesso allo stato completo dell'ambiente in ogni momento.
- **Deterministico** (o stocastico) Lo stato successivo completamente determinato dallo stato corrente e dall’azione eseguita dall’agente.
- **Episodico** (o sequenziale). L'esperienza dell'agente è divisa in "episodi" atomici. Ciascun episodio consiste nell'eseguire una singola azione. La scelta dell'azione in ciascun episodio dipende dall'esisodio stesso.
- **Statico** (o dinamico). L'ambiente è invariato mentre un agente sta deliberando. Si dice semi-dinamico se esso non cambia con il passare del tempo ma il punteggio delle prestazioni dell'agente lo fa
- **Discreto** (o continuo). L'ambiente fornisce un numero limitato di percezioni e azioni distinte. Es. la dama
- **Singolo** (o multi-agente). L'ambiente consente la presenza di un unico agente. Se ci sono più agenti, gli scenati cambiano, negli algoritmi di ricerca qui parleremo di teoria dei giochi. A sua volta questo ambiente si divide in Competitivo e Cooperativo. **Competitivo** è, in un ambiente multi-agente, il comportamento di un agente A è tale da massimizzare/minimizzare la misura di prestazione del comportamento di B (e viceversa). **Cooperativo** in un ambiente multi-agente, è quando due agenti A e B puntano a massimizzare/minimizzare la stessa misura di prestazione.

