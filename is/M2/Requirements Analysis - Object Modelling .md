# Requirements Analysis - Object Modelling 

## Realtà e Modello
- <b>Realtà (R):</b>Cose reali,Persone,Processi che accadono durante un certo tempo,Relazioni tra cose.

- <b>Modello (M):</b>Astrazioni da cose (realmente esistenti o solo pensate),persone,processi e relazioni tra queste astrazioni.

## Perchè i modelli?
Per astrarre dai dettagli nella realtà, in modo da poter trarre conclusioni complicate nella realtà con passi semplici nel modello, per ottenere insight sul passato o sul presente, per fare previsioni sul futuro.

## Che cos'è un "buon" modello?
Le relazioni che sono valide nella realtà R,sono anche valide nel modello M.<br>I: Mappatura di cose reali nella realtà R su astrazioni nel modello M (Interpretation).

- $f_{M}$ :  relazione tra astrazione in M.
- $f_{R}$ :  relazione tra cose reali in R.

<b>In un buon modello il seguente diagramma è commutativo: </b>

<img src = "img/image-22.png" height = 400 width = 600>

## I modelli sono falsificabili
I modelli della realtà non possono essere veri, un modello è sempre un'approssimazione quindi dobbiamo dire "secondo  le nostre conoscenze" o "con le conoscenze di oggi".
- <b>Popper ("Conoscenza Oggettiva"):</b>Possiamo costruire modelli della realtà che sono "veri" fino a quando non troviamo un contro-esempio (Principio di Falsificazione).Questo principio è alla base dello sviluppo software, l'obbiettivo di prototipi , review e system testing è falsificare il sistema software.

## Modelli di modelli di modelli...
La modellazione è relativa.Possiamo pensare a un modello come alla realtà e costruire un altro modello da esso.<br>Lo sviluppo di Sistemi Software è una <b>Trasormazione di Modelli:</b>Analisi,Progettazione,Implementazione,Testing.

## Attività durante la Modellazione degli Oggetti
<b>Obiettivo principale</b>: Trovare le astrazioni importanti, se troviamo astrazioni sbagliate,dobbiamo iterare e correggere il modello.<br>Passi durante la modellazione degli oggetti:

- Identificazioni delle classi
- Trovare gli attributi
- Trovare i metodi
- Trovare le relazioni tra le classi
L'ordine dei passi è secondario, è solo un'euristica;l'iterazione è importante.

## Identificazione delle Classi
- Identificaare i confini del sistema
- Identificare le entità importanti nel sistema.
L'identificazione delle classi è cruciale per la modellazione orientata agli oggetti.<br><b>Assunzione di base:</b>
- Possiamo trovare le classi per un nuovo sistema software (Ingegneria in Avanti - Forward Engineering).
- Possiamo identificare le classi in un sistema esistente (Ingegneria Inversa - Reverse Engineering).

## Oggetto vs Classe

- <b>Oggetto (instance): </b>Esattamente una cosa: 
    - Esempio: Questa lezione di Ingegneria del Software del 16 Aprile dalle 16:00 alle 18:00
- <b>Classe:</b>Descrive un gruppo di oggetti con proprietà simili
    - Esempio: Game,Torunament,car,database.

<b>Diagrammi a Oggetti:</b>Una notazione grafica per modellare oggetti,classi e le loro relazioni

- Diagramma delle Classi: Templete per descrivere molte istanze di dati.Uile per tassonomia,patterns,schemi..

- Diagramma delle Istanze: Un insieme particolare di oggetti correlati tra loro.Utile per discutere scenari,casi di test ed esempi.

## Identificazioni delle Classi
Trovare gli oggetti è il pezzo centrale nella modellazione degli oggetti.<br><b>Approcci:</b>
- <b>Aprroccio al Dominio Applicativo:Chiedere all'esperto di dominio di identificare astrazioni rilevanti</b>
- <b>Approccio Sintatico (oggi):</b>Iniziare con i casi d'uso.Estrarre gli oggetti partecipanti dal flusso di eventi.Usare l'analisi nome-verbo (tecnica di Abbott) per identificare i componenti del modello a oggetti.
- <b>Approccio  ai Design Patterns:</b> Usare design patterns riutilizzabili
- <b>Approccio Basato sui Componenti:</b>Identificare classi di soluzioni esistenti.

 ## Come si trovano le classi?
- Imparare dal dominio del problema: Osservare il cliente.
- Applicare la conoscenza generale del mondo e l'intuizione
- Prendere il flusso di eventi e trovare gli oggetti partecipanti nei casi d'uso
- Provare a stabilire una tassonomia
- Applicare la conoscenza di progettazione: 
    - Distinguere diversi tipi di oggetti.
    - Applicare design patterns
- <b>Eseguire un analisi sintattica della dichiarazione del problema,dello scenario o del flusso di eventi.</b>
- <b>Analisi Testuale  di Abbott (1983), anche chiamata analisi nome-verbo:</b>
    - i <b>nomi</b> sono buoni candidati per le <b>classi</b>
    - i <b>verbi</b> sono buoni candidati per le <b>operazioni</b>

## Modi per trovare gli oggetti

- Indagine sintattica con la tecninca di Abbott:
    -  nel flusso di eventi dei casi d'uso.
- Uso di varie fonti di conoscenza:
    - Conoscenza applicativa (Interviste a utenti ed esperti).

    - Conoscenza di progettazione (Astrazioni riutilizzabili nel dominio della soluzione).

    - Conoscenza generale del mondo (Intuito).

- Formulazione di scenari (Descrizione dell'uso concreto del sistema).

- Formulazione di casi d'uso (Descrizione delle funzioni con attori e flusso di eventi).

## Trovare gli Oggetti Partecipanti nei Casi d'Uso
- Scegliare un <b>caso d'uso</b> e guardare il <b>flusso di eventi</b>
    - Trovare termini che gli sviluppatori o gli utenti devono chiarire
    - Cercare nomi ricorrenti
    - Identificare entità del mondo reale di cui il sistema deve tenere traccia
    - Identificare procedure del mondo reale
    - Identificare fonti o pozzi di dati
    - Identificare artefatti di interfaccia

Essere preparati al fatto che alcuni oggetti sono ancora mancanti e devono essere trovati, ad esempio modellando il flusso di eventi con un diagramma di sequenza.

## Tipi di Oggetti
- <b>Oggetti Entità (Entity Objects):</b>Rappresentano l'informazione persistente tracciata dal sistema
- <b>Oggetti di Confine (Boundary Objects): </b>Rappresentano l'interazione tra l'utente e il sistema
- <b>Oggetti di controllo (Control Objects) :</b> Rappresentano i compiti di controllo eseguiti dal sistema

Avere tre tipi di oggetti porta a modelli più resilienti al cambiamento.
- L'interfaccia camvbia più probabilmente del controllo
- Il controllo cambia più probabilmente del dominio applicativo.
I tipi di oggetto hanno avuto origine in SmallTalk:
-  <b>Model,View,Controller (MVC)</b>.

<img src = "img/image-23.png" height = 400 width = 600>

## Convenzione di Denominazione Raccomandata per i Tipi di Oggetti
Per distinguere i devrsi tipi di oggetto su base sintattica,si raccomandano suffissi.
- Gli oggetti che terminano con il suffisso "_Boundary" sono oggetti di confine.
- Gli oggetti che terminano con il suffisso "_Control" sono oggetti di controllo.
- Gli oggetti entià non hanno alcun suffisso.

## Esempio di Flusso di Eventi
- Il cliente entra in un negozio con l'intenzione di comprare un giocattolo per suo figlio di età n.

- L'aiuto deve essere disponibile entro meno di un minuto.

- Il proprietario del negozio dà consigli al cliente. Il consiglio dipende dalla fascia d'età del bambino e dagli attributi del giocattolo.

- Il cliente seleziona un giocattolo pericoloso che è in qualche modo inadatto al bambino.

- Il proprietario del negozio consiglia una bambola.

## Chi usa il diagramma delle Classi?
<b>Scopo principale</b>: La descrizione delle proprietà statiche di un sistema. <br><b>Il cliente e l'utente</b> spesso non sono interessati ai diagrammi delle classi concentrandosi maggiormente sulla funzionalità.<br><b>L'esperto del dominio applicativo</b> usa i diagrammi delle classi per modellare il dominio applicativo.<br><b>Lo sviluppatore</b> usa i diagrammi delle classi durante tutto lo sviluppo .<br>Ci sono vari tipi di Classi che compaiono nel diagrammi delle classi:

- Classi del dominio applicativo.
- Classi del dominio della soluzione.    

## Dominio applicativo vs dominio della soluzione

-<b> Dominio applicativo:</b> Il dominio del problema (Esempi: servizi finanziari, meteorologia, gestione degli incidenti).


    - Classe del dominio applicativo: Un'astrazione nel dominio applicativo, anche chiamata business object (Esempi: Board game, Tournament).


- <b>Dominio della soluzione:</b> Domini che aiutano nella soluzione dei problemi (Esempi: telecomunicazioni, database, sistemi operativi).


    - Classe del dominio della soluzione: Un'astrazione introdotta per ragioni tecniche, perché aiuta nella soluzione di un problema (Esempi: Tree, Hashtable, Scheduler).

## Il Ruolo dell'Analista
**L'analista è interessato:**
- Alle classi applicative: Le associazioni tra classi sono relazioni tra astrazioni nel dominio applicativo.
- Se l'uso dell'ereditarietà nel modello riflette le tassonomie nel dominio applicativo
    - Definizione Tassonomia: Una gerarchia di astrazioni.
**L'analista non è interessato:**
- Alla firma esatta delle operazioni
- Allle classi di soluzioni

## Progettista (Designer)
Il progettista si concentra sulla **soluzione del problema**, cioè il dominio della soluzione.<br>La progettazione consiste in molti compiti(decomposizione del sottosistema, selezione della piattaforma hardware, sistema di gestione dei dati, ecc.).<br>Un problema  di progettazione importante è la specificazione delle interfacce: il progettista descrive l'interfaccia delle classi e dei sottosistemi.
- **L'obiettivo del progettista è l'usabilità e la riusabilità dell'interfaccia**
    - Design-Usability: Le interfacce sono utilizzabili dal maggior numero possibile di classi all'interno del sistema.
    - Design-Reusability: Definizione di interfacce tali da poter essere utilizzate anche in altri sistemi software.

## Operazioni,Firme o Metodo?

- **Operazione (Operation)**:Una funzione o trasformazione applicata agli oggetti in una classe.Tutti gli oggetti in una classe condividono le stesse operazioni(Fase di Analisi).
- **Firma (Signature)**: Numero e tipi di argomenti,tipo di valore di risultato(Fase di Progettazione degli Oggetti).
- **Metodo(Method)**: Implementazione di un'operazione per una classe(Fase di Implementazione)
    - **Operazione Poliformica**: La stessa operazione si applica a molte classi diverse.

## I diagrammi delle classi fanno sempre parte dei modelli
- **Modello di analisi**:  Modello del dominio applicativo
- **Modelli di Progettazione del Sistema e Progettazione degli Oggetti:** Modello del dominio della soluzione
A seconda del nostro ruolo,guardiamo oggetti e modelli da una prospettiva diversa.Ci sono diverse  interpretazioni  per i diversi cosrtutti UML:
- Associazioni
- Attribuiti
- Ereditarietà

## Modello di Analisi
Il modello di analisi è costruito durante la fase di analisi.<br>Lo **StackHolder principale**: Utente finale,Cliente,Analista.<br>Il diagramma contiene solo classi del dominio applicativo.<br>Il modello di analisi è la base per la comunicazione tra analisti,esperti del dominio applicativo e utenti finali del sistema.


## Modello di Progettazione degli Oggetti (Object design model)
Creato durante la fase di progettazione degli oggetti (a volte chiamato anche specifaction model).<br>Lo **StackHolder principale**:Specificatore di classe,Implementatori di classi e Utenti di classe.<br>I diagrammi delle classi contengono **classi del dominio applicativo e della soluzione**.<br>Il modello di progettazione degli oggetti è la base della comunicazione tra progettisti e implementatori.

