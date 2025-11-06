# UML

## Che cos'è la modellazione?

La modellazione consiste nel cosrtuire un'astrazione della realtà.
Le astrazioni sono semplificazioni perchè:
- ignorano i dettagli irrilevanti
- rappresentano solo quelli rilevanti
Ciò che è rilevante o no dipende dallo scopo del modello.

Essendo che i software stanno diventando sempre più complessi,
- Windowsx XP > 40 milioni di righe di codice
 Quindi un singolo programmatore non è in grado di gestire queste quantità di codice, vi è la necessità di rapprensentazioni più semplici e la modellazioni è un mezzo per affrontare la complessità

 ### Sistemi,Modelli e Viste

 - Un modello è un'astrazione che descrive un sottoinsieme di un sitema
 - Una vista rappresenta aspetti selezionati di un modello
 - Una notazione è un insieme di regole grafiche o testuali per rappresentare le viste

 Esempio: 
 - Sistema: Aereo
 - Modelli: Simulatore di volo, modellino in scala
 - Viste: Tutti i progetti,impianto elettrico, sistema di alimentazione

 <img src = "img/image-1.png" width=400 height=300 >

### Concetti e Fenomeni
Fenomeno:
- Un oggetto nel mondo di un dominio come lo percepisci
Esempio:  la lezione a cui stai partecipando

Concetto:
- Descrive le proprietà dei fenomeni che sono comuni
Esempio: la  lezione di Ingegneria del Software

Il concetto è una 3-upla:
- Nome : per distinguerlo da altri concetti
- Scopo: per detereminare se un fenomeno è membro di un concetto
- Membri: l'insieme dei fenomeni che fanno parte del concetto

### Tipi di Dati Astratti e Classi

Tipo di dato astratto:
- Tipo speciale la cui implementazione è nascosta dal resto del sistema
Classe:
- Un'astrazione nel contesto dei linguaggi orientati agli ogetti

### Domionio Applicativo e Dominio della Soluzione

Dominio Applicativo (Analisi dei Requisiti):
-  L'ambiente in cui opera il sistema

Dominio della Soluzione (System Desgin, Object Design):
- Le tecnologie disponibili per cosrtuire il sistema

## Che cos'è UML?
UML (Unified Modeling Lenguage):
-Uno standard emergente per la modellazione di software orientato agli oggetti.

- Diagrammi dei casi d'uso: Descrivono il comportamento funzionale del sistema visto dall'utente.

- Diagrammi delle classi: Descrivono la struttura statica  del sistema: Oggetti,Attributi,Relazioni.

- Diagrammi di sequenza: Descrivono il comportamento dinamico tra attori e il sistema e tra oggetti del sistema.

- Diagrammi degli stati(Statechart diagrams): Descrivono il comportamento dinamico di un singolo oggetto

- Diagrammi di attività (Activity Diagrams): Modellano il comportamento dinamico di un sistema, in particolare il workflow (digramma di flusso).

### Convenzioni principali di UML
- I rettangoli sono classi o istanza
- Gli ovali sono funzioni o casi d'uso
- Le istanza sono denotate con nomi sottolineati
    -  <u>myWstch: SimpleWatch</u>
    - <u>Joe: Firefighter</u>
- I tipi sono denotati con nomi non sottolineati
    -  SimpleWatch
    - Firefighter
- I diagrammi sono grafi:
    - I nodi sono entità
    - Gli archi sono relazioni tra entità

### Diagrammi dei casi d'uso
Utilizzati durante l'individuazione dei requisiti per rappresentare il comportamento esterno.<br>
Gli attori rappresentano ruoli, cioè un tipo di utente del sistema.<br>
I casi d'uso rappresentano una sequenza di interazione per un tipo di funzionalità.<br>
Il modello dei casi d'uso è l'insieme di tutti i casi d'uso.

### Attori
Un attore modella un'entità che comunica con il sistema:
- Utente
- Sistema esterno
- Ambiente fisico
Un attore ha un nome univoco e una descrizione opzionale
Esempii:
- Passeggero: Una persona sul treno
- Satellite GPS: Fornisce al sistema le coordinate GPS

### Caso d'uso
Un caso d'uso rappresenta una classe di funzionalità fornita dal sistema come un flusso di eventi, esso consiste in:
- nome univoco
- Attori partecipanti
- Condizione di ingresso
- Flusso di eventi
- Condizione di uscita
- Requisiti speciali

### Diagramma dei Casi d'Uso: Esempio

- Nome: Acquista biglietto

- Attore partecipante: Passeggero

- Condizione di ingresso:

    - Passeggero in piedi davanti al distributore di biglietti.

    - Passeggero ha denaro sufficiente per acquistare il biglietto.

- Condizione di uscita:

    - Passeggero ha il biglietto.

- Flusso di eventi:

    - Il Passeggero seleziona il numero di zone da percorrere.

    - Il Distributore visualizza l'importo dovuto.

    - Il Passeggero inserisce denaro, almeno pari all'importo dovuto.

    - Il Distributore restituisce il resto.

    - Il Distributore emette il biglietto.

In questo esempio manca qualcosa  -> Ovvero i casi eccezionali

### La relazione << extends >>

Le relazioni "<< extends >>" rappresentano casi eccezionali o raramente invocati.
<br>
I flussi di eventi eccezionali sono estratti dal flusso di eventi principale per chiarezza.
<br>
I casi d'uso che rappresentano flussi eccezionali possono estendere più casi d'uso.
<br>
La direzione di un relazione "<< extends >>" è verso il caso d'uso esteso.

<img src = "img/image-2.png" width=400 height=300 >



### La relazione << includes >>

Le relazione "<< includes >>" rappresenta un comportamento che viene estratto dal caso d'uso.
<br>
Il comportamento "<< includes >>" viene estratto per il riutilizzo, non perchè sta un'eccezione.
<br>
La direzione di una relazione "<< includes >>"  è verso il caso d'uso che utilizza.

<img src = "img/image-3.png" width=400 height=300 >

## Diagrammi delle Classi
I diagrammi delle classi rappresentano la struttura del sistema, vengono utilizzati:
- durante l'analisi dei requisiti per modellare i concetti del dominio del problema
- durante la progettazione del sistema per modellare i sottoinsiemi e interfacce
- durante la progettazione degli oggetti per modellare le classi.

### Classi
Una classe rappresenta un concetto, essa incapsula lo stato(attributi) e il comportamento (operazioni), ogni attributo ha un tipo e ogni operazione ha una firma (signature), il nome della classe è l'unica informazione obbligatoria.

<img src = "img/image-4.png" width=600 height=300 >

### Instanze
Un instanza rappresenta un fenomeno. <br>
Il nome di un istanza è <u> sottolineato</u> e può contenere la classe dell'istanza, gli attribuiti sono rappresentati con i loro valori

<img src = "img/image-5.png" width=400 height=300 >

### Classi e Istanza
<img src = "img/image-6.png" width=400 height=300 >


### Attori vs Istanze
Qual è la differenza tra un attore, una classe e un'istanza?
<br>
Attore:
- Un'entità esterna al sistema da modellare,che interagisce con il sistema ("Passegero")
<br>
Classe:
- Un'astrazione che modella un'entità nel dominio del problema, deve essere modellata all'interno del sistema ("Utente")
<br>
Oggetto:
- Un'istanza specifica di una classe ("Joe, il passeggero che sta acquistando un biglietto dal distributore automatico").

### Associazione
- Le associazioni denotano relazioni tra classi 
- La molteplicità a un'estremità dell'associazione denota quanti oggetti , l'oggetto sorgente può referenizare

<img src = "img/image-7.png" width=400 height=300 >
<img src = "img/image-8.png" width=400 height=300 >

nell'esempio si nota che:
- un paese ha una sola capitale quindi si dice one-to one 
- un poligono ha più punti, più  punti hanno un solo poligono, quindi si dice one-to-many
- più stockExchange appartengono a più compagnie, e si dice many to many.

### Link e Associazioni
Link e associazioni stasbiliscono relazioni tra oggetti e classi. <br>
Link:
- Una connsessione tra due istanze di oggetti.Un link è come una tupla
- Un link è un istanza di un'associazione
Associazione:
- Fondamentalmente una mappatura biderizionale
- Uno-a-uno,molti-a-uno,uno-a-molti
- Un'associazione descrive un insime di link come una classse descrive un insieme di oggetti.

### Le associazioni UML hanno direzione?
Un'associozione tra due classi è per default una mappatura biderezionale.
<br>
La Classe A può accedere alla Classe B e la Classe B può accedere alla Classe A:<br>

- Entrambe le classi svolgono il ruolo di agente.
<br>

Se si vuole rendere A un client e B un server, si può rendere l'associazione unidirezionale.La freccia punta al ruolo del server:
- Classe A (il "client") accede alla classe B ("il server"). B è anche chiamata navigabile.

## Ruoli
Un "nome di ruole" (roule name) è il nome che identifica in modo univoco un'estermità di un'associazione, è scritto vicino alla linea di associazione, accanto alla classe che svolge il ruolo.

<br>
Quando si usano i nomi di ruolo?
<br>

- Necessario per un associazione tra due oggetti della stessa classe
- Utile anche per distringuere tra due associazioni tra la stessa coppia di classi.

<br>
Quando non si usano i nomi di ruolo?
<br>

- Se c'è solo una singola associazione tra una coppia di classi distinte, i nomi delle classi servono come buoni nomi di ruolo
 
### Ruoli nelle Associazioni
- Ruolo Client:
    - Un oggetto che può operare su altri oggetti che non  viene mai operato da altri oggetti.
- Ruolo Server:
    - Un oggetto che non opera mai su altri oggetti, viene solo operato solo da altri oggetti
- Ruolo Agente:
    - Un oggetto che può sia operare su altri oggetti che essere operato da altri oggetti. Un agente viene solitamente creato per fare del lavoro per conto di un attore o di un altro agente.

### Classi di Associazione
 Sono associazioni che possono avere attributi e operazioni allegati ad esse.

 ### Aggregazione
 Un'aggregazione è un caso speciale di associazione che denota una gerarchia "consiste di".
 <br>
  
L'<b>aggregato</b> è la classe padre, i <b>componenti</b> sono le classi figlio.
<br>

Un rombo pieno denota la composizione,una forma  forte di aggregazione in cui i <b>componenti</b> non possono esistere senza l'aggregato.
<br>

<img src = "img/image-9.png" width=700 height=250 >


### Qualificazione
Il qualificatore migliora l'informazione sulla molteplicità dell'associazione tra le classi.<br> Viene usato per  ridurre la molteplicità 1-a-molti a 1-a-1. <br> Senza qualificazione: una directory ha molti file,un file appartiene ad una sola directory. <br>Con qualificazione:Una directory ha molti file,ciascuno con un nome univoco.

### Ereditarietà
- Le classi figlio ereditano gli attributi e le operazioni della classe padre.
- L'ereditarietà semplifica il modello eliminando la ridondanza

### Modellazione ad Oggetti in Pratica:

<img src = "img/image-10.png" width=500 height=250 >


## Package
- Un package è un meccanismo UML per organizzare elementi in gruppi
- I package sono il costrutto di raggruppamento di base con cui è possibile organizzare i modelli UML per aumentare la leggibilità
- Un sistema complesso può essere decomposto in sottoinsiemi, dove ogni sottoinsieme è modellato come un package.

## Diagrammi di Sequanza UML
- Utilizzati durante l'analisi dei requisiti:
    - per affinare le descrizioni dei casi d'uso
    - Per trovare oggetti aggiuntivi
- Utilizzati duarante la proggettazione del sistema
    - per affinare le interfacce dei sottoinsiemi
- Le Classi sono rappresentate da colonne
- I Messaggi sono rappresentati da frecce
- Le Attivazioni sono rappresentati da rettangoli stretti
- Le Lifeline sono rappresentati da  linee trattegiate

<img src = "img/image-11.png" width=350 height=550 >

### Messaggi annidati
- L'inizio della freccia indica l'attivazione che ha inviato il messaggio 
- Un'attivazione è lunga quanto tutte le attivazioni annidate
- Le frecce tratteggiate orizzontali indicano il flusso dei dati
- Le linee tretteggiate verticali indicano le lifeline

<img src = "img/image-12.png" width=650 height=400 >

### Interazione e condizione

- L'interazione è donotata da un * che precede il nome del messaggio
- La condizione è denotata da un espressione booleana tre parentesi quadre [] prima del nome del messaggio.

<img src = "img/image-13.png" width=650 height=400 >

### Creazione e Distruzione

- La creazione è denotata da una freccia del messaggio che punta all'oggetto
- La distruzione è denotata da un segno X alla fine dell'attivazione di distruzione, essa viene usata per denotare la fine della vita utile di un oggetto.

<img src = "img/image-14.png" width=650 height=400 >

### Riepiligo del Diagramma di Sequenza
- I diagrammi di sequenza UML rappresentano il comportamento in termini di interazioni
- Utili per trovare oggetti mancanti
- Richiedono tempo per la costruzione ma valgono l'investimento
- Complementano i diagrammi delle classi


## Diagrammi degli Stati

Rappresentano il comportamento come stati e transizioni

<img src = "img/image-15.png" width=650 height=400 >


## Diagrammi di Attività

Questo tipo di diagramma mostra il flusso di controllo all'interno di un sistema
- è un caso speciale di diagramma degli stati in cui gli stati sono attività ("funzioni")<br>Due tipi di stati:

- Stato Azione:
    - Non può essere ulteriormente decomposto
    - Avviene "instantaneamente" rispetto al livello di astrazione utilizzato nel modello
- Stato Attività:
    - Può essere ulteriormente decomposto
    - L'attività è modellata da un altro diagramma di attività

## Diagramma degli Stati vs. Diagramma di Attività
<img src = "img/image-16.png" width=650 height=400 >


## Riepilogo UML 
UML fornisce una vasta gamma di notazioni per rappresentare molti aspetti dello sviluppo software
- Linguaggio potente ma complesso
- Può essere frainteso in modo improprio per generare modelli leggibili
- Può essere frainteso quando si usano troppe funzionalità esotiche
<br>

Per ora ci concentriamo su poche notazioni:
- Modello funzionale: Diagramma dei casi d'uso
- Modello oggetto: Diagramma delle classi
- Modello dinamico: Diagramma di sequenza,diagramma degli stati e di attività.

