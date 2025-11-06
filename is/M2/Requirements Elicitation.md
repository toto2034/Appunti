# Requirements Elicitation

Lo sviluppo di un sistema non avviene semplicemente scattando un'istantanea di una scena (dominio).<br>
Ci sono due domande a cui rispondere:
- Come possiamo identificare lo scopo di un sistema?
- La definizione del confine del sistema è cruciale: cosa c'è dentro,cosa c'è fuori al sistema?
Queste domande vengono risposte nel processo dei requisiti che consiste in due attività:

- <b>Elicitazione dei Requisiti:</b>
    - Definizione del sistema in termini compresi dal cliente ("Descrizione del problema").
- <b>Analisi dei Requisiti:</b>
    - Specificazione tecnica del sistema in termini compresi dallo sviluppatore ("Specificazione del Problema").

## Prodotti del Processo dei Requisiti

<img src = "img/image-20.png" width=400 height=300>
Il processo comprende Elicitazione dei Requisiti e Analisi.<br>L'elicitazione contribuisce alla dichiarazione del problema.<br>L'elicitazione e l'Analisi contribuiscono alla <b>Specificazione dei Requisiti</b>, che include:

- Requisiti non funzionali.
- Modello funzionale.

L'analisi producce il <b>Modello di Analisi</b>, che include:
- Modello dinamico
- Modello a oggetti di analisi.

## Specificazione del Sistema vs Modello di Analisi
Entrmabi i modelli si concentrano sui requisiti dal punto di vista dell'utente.
- La specificazione del sistema usa il linguaggio naturale (derivato dalla dichiarazione del problema).
- Il modello di analisi utilizza una notazione formale o semi-formale (ad esempio, un linguaggio grafico come UML).
Il punto di partenza è la dichiarazione del problema (Problem Statement).

## Dichiarazione del Problema (Problem Statement)
Sviluppata dal cliente come descrizione del problema afforntato dal sistema, un altro nome: "Statement of Work".<br>Una buona dichiarazione del problema descrive:
- La situazione attuale
- La funzionalità che il nuovo sistema dovrebbe supportare
- L'ambiente in cui il sistema verrà distribuito
- I deliverable attesti dal cliente
- Le date di consegna
- Un insieme di criteri di accettazione.

## Ingredienti di una Dichiarazione del Problema
- <b>Situazione attuale:</b> Il problema da risolvere
- Descrizione di uno o puù scenari
- Requisiti
    - Requisiti funzonali o non funzionali
    - Vincoli (pseudo requisiti)
- Programma del progetto
    - Principali milestone che prevedono l'interazione con il cliente, inclusa la scadenza per la consegna del sistema.
- Ambiente Target
    - L'ambiente in cui il sistema consegnanto deve eseguire un insieme specificato di test di sistema.
- Criteri di accettazione del Cliente
    - Criteri per i test di sistema.

## Situazione Attuale: Il Problema da Risolvere
Non credo che sia importante nel caso vai a riprenderlo pag 8.

## Tipi di Requisiti
- Requisiti Funzionali:
    - Descrivono le interazioni tra il sistema e il suo ambiente indendentemente dall'implemlementazione
    - Esempio: Un opratore ARENA dovrebbe essere in grado di definire un nuovo gioco.
- Requisiti Non Funzionali:
    - Aspetti visibili all'utente del sistema non direttamente correlati al comportamento funzionale
    - Esempi: Il tempo di risposta deve essere inferiore a 1 secondo, il server ARENA deve essere disponibile 24 ore al giorno.
- Vincoli ("Pseudo Requisiti"):
    - Imposti dal cliente o dall'ambiente in cui il sistema opera.
    - Esempi: Il linguaggio di implementazione deve essere Java; ARENA deve essere in grado di intrfacciarsi dinamicamente ai giochi esistenti.

### Cosa di solito non è presente nei requisiti?
- Struttura del sistema,tecnologia di implementazione.
- Metodologia di sviluppo 
- Ambiente di sviluppo
- Linguaggio di implementazione
- Riutilizzabilità 

### Validazione dei Requisiti
Passo critico nel processo di sviluppo,di solito dopo l'ingegneria o l'analisi dei requisiti, e anche alla consegna.<br>
<b>Criteri di validazione dei requisiti:</b>

- Correttezza: I requisiti rappresentano il punto di vista del cliente.
- Completezza: Sono descritti tutti gli scenari possibili in cui il sistema può essere utilizzato,incluso il comportamento eccezionale.
- Coerenza: Non ci sono requisiti funzionali o non funzionali che si contraddicono a vicenda.
-  Realisimo:  I requisiti possono essere implementati e consegnati.
- Tracciabilià: Ogni funzione di sistema può essere ricondotta a un insieme corrispondente di requisiti funzionali.

### Evoluzione dei Requisiti
Problema: I requisiti cambiano molto velocemente durante l'elicitazione dei requisiti. <br><b>Supporto di strumenti per la gestione dei requisiti:</b>
- Memorizzare i requisiti in una repository condivisa.
- Fornire accesso mulit-utente
- Creare automaticamente un documento di specifica del sistema dalla repository
- Consentire la gestione delle modifiche.
- Fornire tracciabilità durante tutto il ciclo di vita del progetto.

## Tipi di Elicitazione dei Requisiti
<b>Ingengeria Greenfield:</b>

- Lo sviluppo inizia da zero, nessun sistema precedente esiste, i requisiti sono estratti dagli utenti finali e del cliente
- Innescata dalle esigenza dall'utente.+

<b>Re-ingegnaria:</b>

- Riprogettazione e/o re-implementazione di un sistema esistente utilizzando una tecnologia più recente.
- Innescata da un abilitatore tecnologico

<b>Ingenneria dell'Interfaccia:</b>

- Fornire i servizi di un sistema esistente in un nuoco ambiente
- Innescata da un abilitatore tecnologico o da nuove esigenze di mercato.

## Elicitazione dei Requisiti
Attività molto impegnativa.<br>Richiede la collaborazione di persone con background diversi:
- Utenti con conoscenza del dominio applicativo.
- Sviluppatori con conoscenza del dominio della soluzione

<b>Colmare il divario tra utente e sviluppatore:</b>

- Questionari: Chiedere all'utente finale un elenco di domande preeselezionate.
- Analisi delle attività (Task Analysis): Osservare gli utenti finali nel loro ambiente operativo.
- Scenari: Esempio di utilizzo del sistema in termini di una serie di interazioni tra utente e sistema.
- Casi  d'uso: Astrazione che descrive una classe di scenari.

## Perchè Scenari e Casi d'Uso?
Assolutamente comprensibili all'utente.<br>I casi d'uso modellano un sistema dal punto di vista degli utenti(requisiti funzionali):
- Definiscono ogni possibile flusso di eventi attraverso il sistema
- Descrivono l'interazione tra gli oggetti.
Ottimi strumenti per gestire un progetto.I casi d'uso possono costruire la base per l'intero processo di sviluppo:
- Manuale utente
- Progettazione del sistema e degli oggetti.
- Implementazione
- Specifiche di test e test di accettazione del cliente

## Scenari
Una descrizione narrativa di ciò che le persone fanno e sperimentano mentre cercano di utilizzare sistemi e applicazioni informatiche, una descrizione concreta,focalizzata,informale di una singola funzionalità del sistema utilizzata da un singolo attore.Gli scenari possono avere molti usi diversi durante il ciclo di vita del software.<br>Quindi uno scenario è una descrizione sintetica di un evento o di una serie di azioni ed eventi, scritta dal punto di vista dell'utente finale.Uno scenario può includere testo,video,immagini e storyboard.Di solito contiene anche dettagli sul lungo lavoro,situazioni sociali e vincoli di risorse.

### Tipi di Scenari
- Scenario As-is (Com'è):
    - Utilizzato per descrivere una situazione attuale, di solito in progetti di re-ingegneria.L'utente descrive il sistema

-  Scenario Visonario: 
    - Utilizzato per descrivere un sistema futuro, di solito in progetti di ingegneria greenfield e re-ingegneria
    - Spesso non può essere fatto solo dall'utente o dallo sviluppatore

- Scenario di Valutazione:
    - Compiti dell'utente rispetto ai quali il sistema deve essere valutato

- Scenario di Formazione (Training):
Istruzioni passo passo che guidano un utente  novizio attraverso un sistema.

### Progettazione basata su Scenari
Gli scenari possono avere molti usi diversi durante il ciclo di vita del software:
- Elicitazione dei Requisiti: Scenario As-Is,  scenario visonario
- Test di Accettazione del Cliente: Scenario di valutazione
- Disrtibuzione del Sistema: Scenario  di formazione 

<b>Progettazione Basata sui Scenari:</b>L'uso degli scenari in un'attività del ciclo di vita del software.La progettazione basata sui scenari è iterativa.<br>Ogni scenario dovrebbe essere considerato un documento di lavoro da aumentare e rioarganizzare (iterato) quando cambiano requisiti i criteri di accettazione del cliente o la situazione di distribuzione.<br>
La progettazione basata sui scenari si concentra su descrizioni concrete e istanze particolari,non su idee astratte e generiche.
    
- è guidato dal lavoro, non dalla tecnologia
- è open-ended, non cerca di essere completo
- è informale, non formale e rigoroso


### Come troviamo gli sceneri?
Non aspettari che il cliente sia verbale se il sistema non esiste.
- Il cliente comprende il dominio del problema , non il dominio della soluzione,non mettere informazioni anche se il sistema esiste (il motto è: "Ciò che è ovvio non ha bisogno di essere detto").<br>Impegnarsi in un approccio dialettico:
- Tu aiuti il cliente a formulare i requisiti
- Il cliente aiuta te a comprendere i requisiti
- I requisiti evolvono mentre gli scenari vengono sviluppati

### Euristiche per trovare Scenari
Chiedi a te stesso o al cliente:
- Quali sono i compiti primari che il sistema deve eseguire?
- Quali dati l'attore creerà,memorizzerà,cambierà,rimuoverà o aggiungerà nel sistema?
- Quali cambiamenti esterni il sistema deve conoscere?
- Di quali  cambiamenti o eventi l'attore del sistema dovrà essere informato?
Non fare affidamento solo sui questionari


## Casi D'Uso
Un caso d'uso è un flusso di eventi nel sistema,inclusa l'interazione con gli attori.<br>E' avviato da un attore, ogni caso d'uso ha un nome e una condizione di terminazione, la notazione grafica è un ovale con il nome del caso d'uso.<br><b>Modello a Casi d'Uso (Use Case Model):</b>L'insieme di tutti i casi d'uso che specificano la funzionalità completa del sistema.

### Euristiche: Come trovo i casi d'uso?
Selezionare una stretta fetta verticale del sistema (cioè uno scenario).
- Discutere in dettaglio con l'utente per comprendere il suo stile di interazione preferito.
Selezionare una fetta orizzonatle (cioè,molti scenari) per definire l'ambito del sistema.<br>Utilizzare i mock-up come supporto visivo.<br>Per scoprire cosa fa l'utente, una ottima prassi è quella di osservare le attività (Task Observation) invece fare uso di questionari non è un buon metodo.

### Come specificare un Caso d'Uso (Sommario)
- Nome del Caso d'Uso.

- Attori (Descrizione degli attori coinvolti).

- Condizione di Ingresso (Es. "Questo caso d'uso inizia quando...").

- Flusso di Eventi (Linguaggio naturale libero, informale).

- Condizione di Uscita (Es. "Questo caso d'uso termina quando...").

- Eccezioni (Descrivere cosa succede se qualcosa va storto).

- Requisiti Speciali (Elencare requisiti non funzionali e vincoli).

### Relazioni tra Casi d'Uso
Un modello a casi d'uso consiste in casi d'uso e relazioni tra casi d'uso.<br><b>Tipi importanti:</b>
- <b>Dipendenze</b>
    - <b>Include:</b>Un caso d'uso usa un altro caso d'uso
    - <b>Extends:</b>Un caso d'uso estende un altro caso d'uso
- <b>Generalizzazione:</b>Un caso d'uso astratto ha diverse specializzazioni

### << include >>: Decomposizione Funzionale
Problema: Una funzione nella dichiarazione del problema originale è troppo coplessa per essere risolvibile immediatamente.<br>
Soluzione: Descrivere la funzione come l'aggregazione di un insieme di funzioni più sempliciù.Il caso d'uso associato viene decomposto in casi d'uso più piccoli.

### << include >>: Riutilizzo di Funzionalità Esistenti
Problema: Ci sono già funzioni esistenti.Come possiamo riutilizzarle?<br>
Soluzione: La relazione include da un caso d'uso A a un caso d'uso B indica che un'istanza del caso d'uuso A esegue tutto il comportamento descritto nel caso d'uso B ("A delega a B").<br>
Nota: il caso d'uso base non può esistere da solo.Viene sempre chiamato con il caso d'uso fornitore.

### << extend >>: Relazione per i  Casi d'Usp
Probelema:  La funzionalità nella dichiarazione del problema originale deve essere estesa.<br>
Soluzione: Una relazione extend da un caso d'uso A a un caso d'uso B indica che ii caso d'uso A è un estensione del caso d'uso B.<br>
In una relazione extend, il caso d'uso base può essere eseguito senza l'estensione del caso d'uso

### Relazione di Generalizzazione nei casi d'uso
Problema: Hai un comportamento comune tra i casi d'uso e vuoi estrarlo.<br>Soluzione:La relazione di generalizzazione tra i casi d'uo estrae il comportamento comune.I casi d'uso figli ereditano il comportamento del caso d'uso padre e aggiungo o svrascrivono parte del comportamento.

<img src="img/image-21.png" height = 400 width = 600>

### Come scrivere un caso d'uso (Sommario)

- Nome del Caso d'Uso.

- Attori (Descrizione degli attori).

- Condizione di Ingresso ("Questo caso d'uso inizia quando...").

- Flusso di Eventi (Linguaggio naturale libero, informale).

- Condizione di Uscita ("Questo caso d'uso termina quando...").

- Eccezioni (Cosa succede se qualcosa va storto).

- Requisiti Speciali (Requisiti Non Funzionali, Vincoli).

## FURPS+: Categoria di requisiti funzuionali

- <b>Usabilità:</b> La falicità con cui un utente può imparere o operare,preparare input per,e interpretare gli output di un sistema.

- <b>Affidabilità: (Reliability)</b> L'abilità di un sistema o componente di eseguire le funzioni richieste in condizioni stabilite per un periodo specificato.
    - Esempio: Tempo medio tra i guasti,capacità di rilevare guasti,resistenza agli attacchi di sicurezza.

- <b>Prestazioni (Performance): </b> Riguardano gli attributi quantificabili del sistema,come tempo di risposta,througpath,disponibilità e accuratezza.

- <b>Supportabilità (Supportability) </b>: Riguarda la falicità di apportare modifiche al sistema dopo la distribuzione,inclusa adattabilità,manutenbilità  

## FURPS+: Categorie di pseudo requisiti

- <b>Requisiti di Implementazione:</b>Vincoli sull'implementazione del sistema,inclusi strumenti specifici,linguaggi di programmazione o piattaforma hardware.

- <b>Requisiti di Interfaccia:</b>Vincoli imposti da sistemi esterni,inclusi sistemi legacy e formati di interscambio.

-<b>Requisiti Operativi:</b>Vincoli sull'amministrazione e gestione del sistema nell'ambiente operativo

-<b>Requisiti di Packaging:</b>Vincoli sulla consegna effettiva del sistema

-<b>Requisiti Legali:</b>Riguardano questioni di licenza,regolamentazione e cerifacazione.

## Gestione dell'elicitazione dei requisiti
Negozazione delle Specifiche con i clienti:<b>Joint Application Design (JAD)</b>
- Diversi stakeholder (utenti,clienti,sviluppatori) presentano i loro punti di vista,ascoltano,negoziano e giungono a una soluzione accettabile.
- Il documento di specifica dei requisiti è sviluppato dai  diversi stakeholder.

<b>Mantenimento della Tracciabilità</b>

- Seguire il ciclo di vita di un requisito
- Utile per verificare che il sistema sia completo
- Cross-referencing tra documenti, modelli e artefatti di codice, usando strumenti semplici (fogli di calcolo) o strumenti specializzati

## Elicitazione dei Requisiti (Sommario)

L'elicitazione dei requisiti serve a costruire un modello funzionale del sistema che verrà poi utilizzato durante l'analisi per costruire un modello a oggetti e un modello dinamico.


<b>Attività di Elicitazione dei Requisiti:</b> 

- Identificare attori.

- Identificare scenari.

- Identificare casi d'uso.

- Identificare relazioni tra i casi d'uso.

- Rifinire i casi d'uso.

- Identificare requisiti non funzionali.

- Identificare oggetti partecipanti.

Il processo dei requisiti consiste in elicitazione e analisi.

L'attività di elicitazione è diversa per Greenfield Engineering, Reengineering, Interface Engineering.<br>

Scenari: Ottimo modo per stabilire la comunicazione con il cliente; <br>Tipi diversi: As-Is, visionario, valutazione e formazione;<br> I casi d'uso sono l'astrazione degli scenari.

- La pura decomposizione funzionale è negativa: 
    - Porta a codice non manutenibile.

- La pura identificazione di oggetti è negativa: 
    - Può portare a oggetti, attributi o metodi sbagliati.

- La chiave per un'analisi di successo: 

    - Iniziare con i casi d'uso e poi trovare gli oggetti partecipanti.

    - Se qualcuno chiede "Cos'è questo?", non rispondere subito. Restituire la domanda o osservare l'utente finale: "A cosa serve?"