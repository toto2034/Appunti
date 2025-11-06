# Project Organization and Communication

## La Comunicazione è importante
Nello sviluppo di grandi sistemi, si spende più tempo a comunicare che a programmare.<br> UML consente ai partecipanti al progetto di cosrtuire modelli e comunicare su di essi, tuttavia ,i modelli non sono l'unica informazione necessaria quando si comunica in un progetto.<br>Un ingegnere del software deve imparare le <b>soft skill</b>(abilità trasversali): scrittura tecnica,lettura della documentazione,comunicazione,collaborazione,gestione.presentazioni.<br> In questo corso:
- Gestione: Condurre una riunone di team
- Presentazione: Presentare un aspetto importante del proprio progetto durante la fase di sviluppo.
- Collaborazione: Negoaziare i requisiti con il cliente e ccon i membri del proprio team e di altri team.
-  Scrittura Tecnica: Scrivere parte della documentazione del prorpio progetto.

## Componenti del Progetto

- Prodotto di Lavoro(Work product): Qualsiasi elemento prodotto del progetto, come un pezzo di codice,un modello o un documento.I prodotti di lavoro realizzati per il cliente sono chiamati <b>deliverables</b>.
- Programmazione (Schedule):Specifica quando il lavoro sul progetto deve essere completato.
- Partecipante: Qualsiasi persona partecipante a un progetto, chiamata anche membro del progetto.
- Compito (Task): Il lavoro che deve essere svolto da un partecipante al progetto per creare un prodotto di lavoro.

## Panoramica sui progetti
Definizione del Progetto: Formale (es contratto firmato) o informale (es promessa di fare qualcosa).<br>Ci sono vari tipi di progetto, dipendono principalmente dai deliverables ad esempio progetto software,progetto di sistema. <br> Dimensione del progetto: da piccolo a grande. <br> Stati del progetto:
- Inizio -> si assegna il compito
- Definizione -> si definisce l'ambito
- Stato Stazionario -> si sviluppa il sistema
- Terminazione -> si consegna il sistema

## Comunicazione di Progetto

Comunicazione Pianificata (Planned): aiuta a diffondere informazioni che i partecipanti sono tenuti a realizzare
- Ispezione di problemi 
- Riunioni di stato
- Revisioni tra parti
- Revisioni del cliente e del progetto
- Rilasci

Comunicazione non Pianificata: aiuta ad affrontare crisi ed esigenze inattese
- Richiesta di chiarimento
- Richiesta di modifica
- Risoluzione dei problemi

## Fase di avvio del progetto
- Partecipanti alla runione di kick-off: i partecipanti ascoltano il cliente riguardo al problema da risolvere e all'ambiente del sistema da sviluppare.

- Formare un Team: i partecipanti sono assegnati a un team in base alle loro compotenze e interessi.

- Partecipare a sessioni di formazione: I partecipanti che non possiedono le competenze ricevono una formazione aggiuntiva.

- Unire l'infrastruttura di comunicazione: L'infrastruttura di comunicazione del progetto supporta eventi di comunicazione sia pianificati che non pianificati.

- Estendere l'infrastruttura di comunicazione: Vengono stabiliti ulteriori bacheche e portali team.

- Partecipare alla prima riunione di stato del team: i partecipanti sono istruiti a condurre riunioni di stato, registrare le informazioni di stato e diffondere agli altri membri del progetto.

- Comprendere la pianifacazione delle revisioni: La pianificazione delle revisioni contiene una serie di tappe importanti, per comunicare i risultati del progetto tramite revisioni al project menager e al cliente.

## Organizzazione Basata sui Team

- Team: Piccolo gruppo di partecipanti che lavorano sulla stessa attività o compito.
- Gruppo: Insieme di persona a cui è assegnato un compito comune, ma che lavorano individualmente senza dover comunicare per completare la loro parte del compito.
- Comitato: Composto da persone che si riuniscono per rivedere e criticare problemi e proporre azioni.

## Tipo di interazione

Reporting: Utilizzato per la segnalazione di informazioni di stato
- Esempio: uno sviluppatore riferisce a un altro che un'API è pronta

Decisione: Utilizzato per la propagazione delle decisioni  
- Esempio: un team leader decide che uno sviluppatore deve pubblicare un API

Comunicazione: Utilizzato per lo scambio di tutti gli altri tipi di informazioni
- Esempio: Scambio di requisiti o modelli di progettazione.

## Problemi dell'Organizzazione Gerarchica

La struttura di reporting è gerarchica: le informazioni di stato e di decisione sono unidirezionali:
- Le decisioni sono prese alla radice e passate alle foglie
- Lo stato è generato alle foglie e riportato alla radice.
<br>

<img src = "img/image-17.png" width=600 height=300>

Molte decisioni tecniche devono essere prese localmente dagli sviluppatori ma dipendono da informazioni provenienti da altri team.<br>Usare la struttura di reporting per la comunicazione ralletta significativamente il processo decisionale.

- Soluzione: Scambiare informazioni tramite una struttura di comunicazione aggiuntiva che permetta ai partecipanti di comunicare tra loro.
    - Spesso la comunicazione è delegata a uno sviluppatore chiamato <b>liaison</b> responsabile di trasferire le informazioni avanti e indietro
    - Se agli sviluppatori è permesso comunicare tra di loro la struttura di comunicazione prende il nome di <b>peer-based</b>.

## Ruoli (Roles)

- Un ruolo definisce l'insieme dei compiti tecnici e manageriali attesi da un partecipante o un team.

- In un'organizzazione basata sui team, i compiti sono assegnati a una persona o a un team tramite un ruolo.

Tipi di ruoli in un progetto software:

- Ruoli di Gestione: riguardano l'ogranizzazione e l'esecuzione del progettio entro i vincoli

- Ruoli di Sviluppo: Riguardano la specificazione, la progettazione e la costruzione dei sottoinsiemi.Includono l'analista,l'architetto di sistema,il progettista di oggetti e implementatore e tester.

- Ruoli Cross-funzionali: riguardano il coordinamento tra i team

- Ruoli di Consulente: riguardano la fornitura di supporto temporaneo per i partecipanti

<img src = "img/image-18.png" width=600 height=400>

## Compiti e prodotti di lavoro (Task and Work Poduct)

Un compito (task) è un'assegnazione di lavoro ben definita per un ruolo.
- il project manager o il team leader assegna un compito a un ruolo
- il partecipante svolge il compito e il menager ne monitora l'avanzamento
- Gruppi di compiti prendono il nome di <b>attività (activities)</b>

Un prodotto di lavoro (work product) è un elemento tangibile che risulta da un compito,ad esempio un documento,  un pezzo di codice sorgente ecc.<br> Qualisasi prodotto di lavoro da consegnare al cliente prende il nome di <b>deliverable</b>

## Pacchetti di Lavoro (Work Packages)
La specifica del lavoro da compiere per completare un compito o un'attività è descritta in un <b> pacchetto di lavoro </b>. </br> Questo include:  
- Nome del compito e descrizione del compito
- Risorse necessarie per eseguire il compito
- Dipendenza degli input e degli output

## Programmazione (Schedule)

Una programmazione è la mappattura dei compiti sul tempo: a ogni compito sono assegnati tempi di inizio e fine.<br>Questo permette di pianificare le scadenze per i singoli deliverables.<br>Le due notazioni diagrammatiche più usate sono i diagrammi <b>PERT e Gantt</b>.
- Un diagramma di Gannt è un grafico a barre dove l'asse orizzontale rappresenta il tempo e quella verticale rappresenta i deversi compiti da svolgere.
- Un diagramma di PERT rappresenta la programmazione come un grafo aciclico di compiti.
    - viene calcolato il percorso critico (critical path), che rappresenta il percorso più lungo attraverso il grafo.
    - La lunghezza del percorso critico corrisponde alla tempistica più breve possibile
    - Un ritardo in un compito sul percorso critico si traduce in un ritardo nel progetto complessivo.

## Comunicazione di Progetto: Definizioni
<b>Modalità di comunicazione:</b>
Tipo di scambio di informazioni che obiettivi e ambito definiti

- Pianificata (Scheduled):comunicazione pianificata
- Basata sull'Evento (Event Driven): comunicazione non pianificata

<b>Meccanismo di comunicazione</b>
Strumento o procedura che può essere utilizzato per trasmettere informazioni.

- Sincrono: mittente e destinatario sono disponibili nello stesso momento
- Asincrono: mittente e destinatario non comunicano allo stesso momento

### Modalità di comunicazione pianificata (Scheduled)

<b>Definizione del problema (Problem Definition):</b>
- Obiettivo: presentare obiettivi, vincoli e requisiti
- Esempio: Presentare al Cliente
- Programmazione: Di solito all'inizio di un progetto

<b>Revisione del Progetto:</b> Focus sul modello di sistema
- Obiettivo: Valutare lo stato e rivedere il modello di sistema, la scomposizione del sistema e le interfacce dei sottoinsiemi.
- Esempio: Revisione di Analisi,Revisione di progettazione di Sistema.
- Programmazzione: Attorno a tappe importanti e deliverables del progetto.

<b>Revisione del Cliente:</b>Focus sui requisiti
- Obiettivo: Informare il cliente , concordare modifiche ai requisiti.
- Esempio: Revisione del Cliente
- Programmazzione: Di solito dopo la fase di analisi.

<b>Revisione tra Pari</b>

- Walkthrough (Informale) 
    - Obiettivo: Aumentare le qualità del sottosistema
    - Esempio: Lo sviluppatore presenta il sottosistema ai membri del team,informale,peer-to-peer
    - Programmazzione: Da pianificare da parte di ogni team
- Ispezione (Formale)
    - Obiettivo: Conformità dei requisiti
    - Esempio: Test di accettazione del cliente
    - Programmazzione: Da pianificare dalla gestione del progetto

<b>Revisione dello Stato</b>

- Obiettivo: Trovare deviazioni della programmazione e correggerle o identificare nuovi problmei
- Esempio: Sezione stato nella regolare riunione settimanale del team.
- Programmazzione: Programmata ogni settimana    

<b>BrainStorming</b>
- Obiettivo: Generare e valutare un gran numero di soluzioni del problema
- Esempio: Sezione di discussione nella regolare riunione settimanale del team
- Programmazzione: Programmato ogni settimana

<b>Rilascio (Release)</b>
- Obiettivo: Stabilire la baseline (punto di riferimento) del risultato di ogni attività di sviluppo software
- Esempio: Piano di Gestione del Progetto Software (SPMP), Documento di Analisi dei Requisiti (RAD), Documento di Progettazione di Sistema (SDD), Documento di Progettazione di Oggetti (ODD), Manuale di Test (TM), Manuale Utente (UM).
- Programmazzione: Di solito dopo ogni fase.

<b>Revisione post-mortem</b>

- Obiettivo: Descrivere le lezioni apprese
- Programmazzione: Programmata alla fine del progetto.

### Modalità di comunicazione basata sull'evento (Event Driven)

<b>Richiesta ddi chiarimento</b><br>
Il grosso della comunicazione tra sviluppatori,clienti e utenti.

- Esempio: Uno sviluppatore può richiedere un chiarimento su una fase ambigua nella dichiarazione del problema.

<b>Richiesta di modifica</b><br>
Un partecipante segnala un problema o propone una soluzione.<br>Le richieste di modifica sono spesso formalizzate quando la dimensione del progetto è sostanziale.

- Esempio:Un parteccipante segnale un problema all'aria condizionata in aula e suggerisce una modifica.

<b>Risoluzione di Problemi</b><br>
Seleziona una singola soluzione a un problema oer il quale sono state proposte diverse soluzioni.<br>Utilizza una base di problemi per raccogliere problemi e proposte.


## Ruoli in Riunione
- Facilitatore Principale: Responsabile dell'organizzazione e della guida dell'esecuzione, scrive e  distribuisce l'agenda.
- Verbalizzatore: Responsabile della regesistrazione della riunione,  identifica e distribuisce gli elementi di azione e i problemi.
- Cronometrista: Responsabile di tenere traccia del tempo.

### Meccanismi di Comunicazione Sincrona

| Meccanismo | Supporta | Pro | Contro |
| :--- | :--- | :--- | :--- |
| **Conversazione in corridoio** (faccia a faccia) | Conversazioni non pianificate, Richiesta di chiarimento, Richiesta di modifica | Economico ed efficace per risolvere problemi semplici | Informazioni importanti possono essere perse, possono verificarsi incomprensioni quando la conversazione viene riferita ad altri |
| **Riunione** (faccia a faccia, telefono, videoconferenza) | Conversazioni pianificate, Revisione del cliente, Revisione del progetto, Revisione dello stato, Revisione tra pari, Revisione post-mortem, Brainstorming, Risoluzione di problemi | Meccanismo efficace per la risoluzione di problemi e la creazione di consenso | Costo elevato (persone, risorse); difficoltà nella gestione e nell'ottenimento di risultati efficaci |
| **Questionario e Interviste Strutturate** | Definizione del problema, Revisione post-mortem | Consente di chiarire molte incomprensioni durante l'elicitazione dei requisiti a basso costo per l'utente | Difficile da progettare |
| **Groupware Sincrono** | Conversazione non pianificata, Revisione del cliente, Revisione del progetto, Revisione tra pari, Brainstorming, Risoluzione di problemi | Le persone comunicano nello stesso momento pur essendo in luoghi diversi | Difficile coordinare gli utenti |

### Meccanismi di Comunicazione Asincrona

| Meccanismo | Supporta | Pro | Contro |
| :--- | :--- | :--- | :--- |
| **E-Mail** | Rilascio, richiesta di modifica, brainstorming | Ideale per modalità di comunicazione basate sull'evento e annunci | L'e-mail estrapolata dal contesto può essere facilmente fraintesa, inviata alla persona sbagliata, persa o non letta dal ricevente |
| **Newsgroups** | Rilascio, richiesta di modifica, brainstorming | Adatto per notifica e discussione tra persone che condividono un interesse comune; economico (shareware disponibile) | Controllo degli accessi primitivo (spesso, si è dentro o fuori) |
| **World Wide Web** | Rilascio, richiesta di modifica, ispezioni | Fornisce all'utente una metafora ipertestuale: I documenti contengono collegamenti ad altri documenti | Non supporta facilmente documenti in rapida evoluzione |
| **Lotus Notes** | Rilascio, richiesta di modifica, brainstorming | Fornisce eccellenti meccanismi di controllo degli accessi e replicazione dei database | Formato proprietario, costoso |