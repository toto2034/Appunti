# Requirements Analysis - Dynamic Modelling

## Come si trovano le classi?
Come abbiamo già visto e stabilito le seguenti fonti:
- Analisi del dominio applicativo: Parlare con  il cliente per identificare le astrazioni.
- Applicazione della conoscenza generale del mondo e dell'intuizione
- Scenari: Formulazione in linguaggio naturale di un uso concreto del sistema
- Casi d'uso: Formulazione in linguaggio naturale delle funzioni del sistema
- Metodo Abbot.
Ora mostriamo come identificare le classe dai modelli dinamici:
- Gli **eventi** in un diagramma di sequenza, così come le azioni e le attività nei diagrammi state chart,sono candidati per le operazioni pubbliche nelle classi.
- Le **linee di attività (Activity lines)** nei diagrammi di sequenza sono anche candidati per gli **oggetti** 

## Modellazione Dinamica con UML
- **Diagrammi per la modellazione dinamica:**
    - I **diagrammi di interazione** descrivono il comportamento dinamico tra gli oggetti.
    -I **diagrammi state chart** descrivono il comportamento dinamico di  un singolo oggetto.

- **Diagrammi di Interazione:**

    - **Diagrammi di Sequenza (Sequence Diagram)**: Comportamento dinamico di un inisieme di oggetti disposti in sequenza temporale.Buono per specifiche in tempo reale e scenari complessi.
    - **Diagramma di Collaborazione(Collaboration Diagram)**: Mostra la relazione tra gli oggetti.Non mosrta il tempo.

- **Diaggramma State Chart**: 
    - Una macchina a stati che descrive la risposta di un oggetto di una data classe al ricevimento di stimoli esterni (**Event**) 
    - **Diagramma di Attività (Activity Diagram)**: Un tipo speciale di diagramma state chart,dove tutti gli stati sono stati di azione.

    ## Modellazione Dinamica

    Definizione di modello dinamico:
    - Una collezione di più diagrammi state chart,un diagramma state chart per ogni classe con un importante comportamento dinamico.

    Scopo:
    - Rilevare e fornire **metodi** per il modello a oggetti.

    Come lo facciamo?
    - Iniziare con un caso d'uso o uno scenario
    - Modellare l'interazione tra oggetti -> **diagramma di sequenza**.
    - Modellare il comportamento dinamico di un singolo oggetto -> **diagramma state chart** 

    ## Che cos'è un Evento?
    Qualcosa che accade in un punto nel tempo.
    **Relazione degli eventi tra loro:**
    - Casualmente correlati: Prima,Dopo.
    -  Casualmente non correlati: Concorrenti.

Un evento manda informazioni da un oggetto a un altro.Gli eventi possono essere raggruppati in classe di eventi con una struttura gerarchica."Evento" è spesso usato in due modi:
-  **istanza di una classe di eventi**
- **Attributo di una classe di eventi**

## Diagramma di Sequenza (Sequence Diagram)
Dal flusso di eventi nel caso d'uso o scenario si procede al diagramma di sequenza, esso è  una descrizione grafica degli oggetti partecipanti in un caso d'uso o scenario utilizzando una notazione DAG (direct acyclic graph - grafo aciclico diretto).

**Relazione con l'identificazione degli oggetti:**
- Oggetti/classi sono già stati identificati durante la modellazione degli oggetti.
- Gli oggetti sono identificati come risultato della modellazione dinamica.

**Euristiche:**
- Un evento ha sempre un mittente e un ricevente.
- La rappresentazione dell'evento è talvolta chiamata messaggio.
- Trovarli per ogni evento -> Questi sono gli oggetti partecipanti al caso d'uso.

## Esempio Sequence Diagam
**Flusso di eventi nel caso d'uso "Get SeatPosition" (Ottieni Posizione del Sedile):**

- 1) Stabilire la connessione tra smart card e computer di bordo.

- 2) Stabilire la connessione tra computer di bordo e sensore per il sedile.

- 3) Ottenere la posizione attuale del sedile e memorizzarla sulla smart card.

Quali sono gli oggetti?

<img src = "img/image-24.png" width=600 height=400>

## Euristiche per i Diagrammi di Sequenza
- **Layout:**
    - 1ª colonna: Dovrebbe corrispondere all'attore che avviato il caso d'uso
    - 2ª colonna: Dovrebbe essere un oggetto di confine(boundary object).
    - 3ª colonna: Dovrebbe essere l'oggetto di controllo che gestisce il resto del caso d'uso.

- **Creazione:**
    - Gli oggetti di controllo vengono creati all'avvio di un caso d'uso.
    - Gli oggetti di cofine vengono creati dagli oggetti di controllo.

- **Accesso:**
    - Gli oggetti entità (entity object) sono acceduti da oggetti di controllo e di confine.
    - Gli oggetti entità non dovrebbero mai chiamare oggetti di confine o di controllo:Ciò rende più facile condividere gli oggetti entità tra i casi d'uso e renderli resilienti ai cambiamenti indotti dalla tencologia negli oggetti di confine.

## Fork Diagram
Gran parte del comportamento dinamico è posto in un **singolo oggetto**, di solito l'oggetto di controllo.Esso conosce tutti glli altri oggetti e spesso li usa per domande e comandi diretti


<img src = "img/image-25.png" width=600 height=400>

## Stair Diagram (Diagramma a Scala)
Il comportamento dinamico è **distribuito**.Ogni oggetto delega una certa responsabilità ad altri oggetti.Ogni oggetto conosce solo pochi altri oggetti e sa quali oggetti possono aiutare con un un comportamento specifico


<img src = "img/image-26.png" width=600 height=400>

## Fork o Stair
Quali di questi due diagrammi dovrebbe essere scelto?<br>I fan dell'orientamento agli oggetti sostengono la struttura a scala poichè più la responsabilità è distribuita meglio è.<br>Tuttavia questo non è sempre vero.
**Euristiche migliori:**
- **Struttra di controllo decentralizzata (Scala):**
    - Le operazioni hanno una forte connessione.
    - Le operazioni saranno sempre eseguite nello stesso ordine.
- **Struttura di controllo centralizzata (Fork)**(migliore supporto per il cambiamento):
    - Le operazioni possono **cambiare ordine**
    -  Nuove operazioni possono essere inserite come risultato di nuovi requisiti.


## Diagramma Statechart
Grafo in cui i nodi sono **STATI** e i cui archi diretti sono **TRASAZIONI** etichettate con nomi di eventi.<br>Distinguiamo i due tipi di operazioni statechart:
- **Attività (Activity):**Operazione che richiede tempo per essere completata.Associata agli stati.
- **Azione (Action):**Operazione istantanea.Associata agli eventi o associata agli stati:Entry,Exit,Internal Action.
Un diagramma statechart mette in relazione eventi e stati per **una sola classe**.

## State (Stato)
Un'astrazione degli attributi di una classe, lo stato quindi è l'aggregazione di diversi attributi di una classe.<br>Fondamentalmente è una **classe di equivalenza** di tutti quei valori di attributo e link che non hanno  bisogno di essere distinti per quanto riguarda la struttura di controllo del sistema.<br>Esempio: Stato di una banca: Una banca è solvente o insolvente.<br>Lo stato ha una durata.

<img src = "img/image-27.png" width=600 height=400>

## Diagramma di Stato Annidato (Nested State Diagram)

Le attività negli stati sono elementi composti che denotano altri diagrammi di stato di livello inferiore.<br>Un diagramma di stato di livello inferiore corrisponde a una sequenza di stati ed eventi di livello inferiore che sono invisibili nel diagramma di livello superiore.<br>Insiemi di sottostati in un diagramma di stato annidato denotano un superstato e sono racchiusi da una grande scatola arrotondata, anche chiamata contorno.

## Superstati
**Obiettivo:**
- Evitare i spaghetti modeles.
- Ridurre il numero di linee in un digramma di stato.
Le transizioni verso altri stati da un superstato sono eridate da tutti i sottostati (**eriditarietà di stato**):
- ... eccetto nel caso di transizioni che devono essere eseguite alla fine delle attività associate allo stato (come nell'esempio precedente).

## Modellazione della Concorennza (Concurrency)
**Ci sono due tipi di concorrena:**
- 1) Concorrenza di sistema (System concurrency):
    - Lo stato del sistema complessivo è l'aggregazione di diagrammi di stato,uno per ogni oggetto.Ogni diagramma di stato è in esecuzione concorrente con gli altri.
- 2) Concorrenza di oggetto (Object concurrency):
    - Un oggetto può essre partizionato in  sottoinisiemi di stati (attributi e link) in modo tale che ognuno di essi abbia il proprio sottodiagramma.
    - Lo stato dell'oggetto consiste in un insieme di stati: uno stato da ogni sottodiagramma.
    - I diagrammi di stato sono divisi in sottodiagrammi da linrr trattegiate.

<img src = "img/image-28.png" width=600 height=400>

## Diagramma State Chart vs. Diagramma di Sequenza

- I diagrammi State chart aiutano a identificare:

    - Cambiamenti in un singolo oggetto nel tempo.

- I diagrammi di sequenza aiutano a identificare:

    - La relazione temporale tra gli oggetti nel tempo.

    - La sequenza di operazioni come risposta a uno o più eventi.

## Modellazione Dinamica delle Interfacce Utente

- I diagrammi Statechart possono essere utilizzati per la progettazione delle interfacce utente.Chiamato anche **Percorso di Navigazione (Navigation Path)**.
- **Stati:** Nome delle schermate.
    - Il layout grafico delle schermate associate agli stati aiuta quando si presenta il modello dinamico di un'interfaccia utente.
- **Attività/azioni** sono mostrate come punti elenco sotto il nome della schermata.Spesso viene mostrata solo l'azione di uscita.

- **Transazioni di stato:**Risultato dell'azione di uscita  (Esempi: Tasto cliccato, Selezione di menu, Movimenti del cursore)


## Quando un modello è dominante?
- **Modello a oggetti:**il sistema ha oggetti con uno stato non banale
- **Modello dinamico:** il modello ha molti tipi di eventi: input,output,eccezioni,errori,ecc..
- **Modello funzionale:** il modello esegue transformazioni complicate
- Quale di questi modelli è dominante nei seguenti tre casi? 

    - Compilatore.

    - Sistema di database.

    - Programma di foglio elettronico (Spreadsheet program).

##  Dominanza dei modelli

- **Compilatore:**
    - Il modello funzionale è più importante.
    - Il modello dinamico è banale perchè c'è solo tipo di input e poche uscite.
- **Sistemi DataBase:**
    - il modello a oggetti è il più importante
    - il modello funzionale è banale,perchè lo scopo delle funzioni è di solito memorizzare,organizzare e recuperare dati.
- **Programma di foglio elettronico (Spreadsheet program).**
    - il modello funzionale è il più importante
    - il modello dinamico è interessante se il programma consente calcoli su una cella.
    - il modello a oggetti è banale,perchè i valori del   spreadsheet sono banali e non possono essere strutturati ulteriormente. L'unico oggetto interessante è la cella.

## Correttezza, Completezza e Coerenza

- La **Verifica** è un controllo di equivalenza tra la trasformazione di due modelli.

- La **Validazione** è diversa. Dobbiamo confrontare un modello con la realtà. 
    - La "Realtà" può anche essere un sistema artificiale, come un sistema legacy.


- La validazione è un passo critico. I requisiti dovrebbero essere validati con il cliente e l'utente.


- **Tecniche:** Review formali e informali.

- La validazione dei requisiti comporta i seguenti controlli: Correttezza, Coerenza, Completezza, Ambiguità, Realismo

## Coerenza, Completezza, Ambiguità

- **Coerenza (Consistency):**

    - Identificazione di "fili incrociati" tra le classi.

    - Denominazione di classi, attributi, metodi.


- **Completezza (Completeness):**

    - Identificazione di associazioni pendenti (dangling associations) (associazioni che puntano a nulla).

    - Identificazione di classi definite due volte.

    - Identificazione di classi mancanti (a cui si fa riferimento in un sottosistema ma non definite da nessuna parte).


- **Ambiguità (Ambiguities):**

    - Errori di ortografia dei nomi.

    - Classi con lo stesso nome ma significati diversi.