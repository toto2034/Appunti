# Software Configuration Management

## Perchè la gestione della configurazione del Software?

Il probleme:

- Più persone devono lavorare sul software in evoluzione
- Deve essere supportata più di una versione del software:
    - sistemi rilasciati
    - sistemi configurati su misura
    - sistemi in fase di sviluppo
Il software deve essere eseguito su diverse macchine e sistemi operativi.
- La gestione della configurazione del software:
    - gestisce i sistemi software in evoluzione
    - controlla i costi nell'apportare modifiche a un sistema.

## Che cos'è la gestione della configurazione del software?
- Definizione: Un insieme di discipline di gestione all'interno del processo di ingegneria del software per sviluppare una baseline. 
- Descrizione: La gestione della configurazione del software comprende  le discipline e le tecniche per avviare,valutare e controllare i cambiamenti ai prodotti software durante e dopo il processo di ingegneria del software.
- Standard: 
    - IEEE 828-2005: Piani di Gestione della Configurazione del Software.
    -  IEEE 1042-1987: Guida alla Gestione della Configurazione del Software (Archiviata)

## Attività di gestione della configurazione
- Identificazioni degli elementi di configurazione:
    - modellazione del sistema come un insieme di comportamenti in evoluzione.
- Gestione delle promozioni:
    - la creazioni di versioni per altri sviluppatori
- Gestione dei rilasci:
    - la creazione di versioni per i clienti e gli utenti
- Gestione dei cambiamenti:
    - la gestioni.l'approvazione e il tracciamento delle richieste di cambiamento.
- Gestione dei branch:
    - la gestione degli sforzi di sviluppo concorrente
- Gestione delle varianti:
    - la gestione delle versioni destinate a coesistere
- Non ci sono regole fisse:
    - Le attività SCM (Software Configuration Management) vengono solitamente eseguite in modi diversi
    - Ciò dipende da tipo  di progetto e dalla fase del ciclo di vita.

## Terminologia
Ora definiamo i seguenti termini:
- Elemento di configurazione (Configuration Item)
- Baseline
- Directory SCM
- Versione
- Revisione
- Rilascio
La definizione dei termini segue lo standard IEEE

### Elemento di configurazione (Configuration Item)

Gli elementi di configurazione del software non sono solo segmenti di codice di programma, ma tutti i tipi di documento in base allo sviluppo, ad esempio:
- tutti i tipi di file di codice
- dirver per i test
- documenti di analisi di progettazione
- manuali per l'utente o lo sviluppatore
- configurazioni di sistema.

### Individuazione degli elementi di configurazione
I progetti di grandi dimensioni producono in genere migliaia di entità, che devono essere identificate in modo univoco.<br>Qualsiasi entità gestita nel processo di Ingegneria del software può potenzialmente essere posta sotto controllo della gestione della configurazione, ma non tutte le entità devono essere sotto il controllo della gestione della configurazione per tutto il tempo.<br>Due Problemi:
- Cosa:
    - Cosa dovrebbe essere sotto controllo della configurazione?
- Quando:
    - Quando si inizia a porre le entità sotto controllo della configurazione?
iniziare troppo presto con gli CI, si ha troppa burocrazia, introdurli troppo tardi si finisce nell caos.

 <img src = "img/image-19.png" width=400 height=300 >
 
### Versione vs Revisione vs Rilascio

Versione:
- Lo stato di un elemento di configurazione o di un aggregato di configurazione in un punto ben definito nel tempo.
- Di solito è associataa a una compilazione o ricompilazione completa dell'elemento.
- Versioni diverse di solito hanno funzionalità diverse.

Revisione:
- Modifica a una versione che corregge solo errori nella progettazione/codice, ma non influisce sulla funzionalità

Rilascio:
- Una versione che è stata resa disponibile esternamente
- La disrtibuzione formale di una  versione approvata.

### Baseline

Una specifica o un prodotto che è stato formalmente revisionato e concordato dalla gestione responsabile,che da quel momento funge da base per ulteriori sviluppi e può essere modificato solo attraverso procedure formali di controllo dei cambiamenti.

- Esempi:
    - Baseline A: Tutte le API sono state completamente definite, i corpi dei metodi sono vuoti.
    -  Baseline B: Tutti i metodi di accesso ai dati sono implementati e testati.
    - Baseline C: L'interfaccia utente grafica (GUI) è implementata

### Approfondimento sulla Baseline

Man mano che i sistemi vengono sviluppati, viene creata una serie di baseline, di solito dopo una revisione:
- <b>Baseline di Sviluppo</b>: (Elementi di Configurazioni: RAD)
    - Obiettivo: Coordinare le attività di Ingegneria
- <b>Baseline Funzionali</b>: (Elementi di configurazione: primo prototipo)
    - Obiettivo: Ottenere le prime esperienze del cliente con il sistema funzionale
- <b>Baseline di Prodotto</b>
    - Obiettivo: Coordinare le vendite e il supporto cliente

Esistono molti schiemi di denominazione per le baseline (1.0,3.14159,6.01a,...).<br>
Uno schema a 3 cifre è abbastanza comune:
- .  10. Rilascio(Cliente)
- .3. Versione(Sviluppatore)
- .6 Revisione(Sviluppatore)

### Gestione dei cambiamenti
La gestione dei cambiamenti è la gestione delle richieste di cambiamento.Una richiesta di cambiamento porta alla creazione di un nuovo rilascio.<br><b>Processo di cambiamento generale : </b>
- Il cambiamento viene richiesto (può essere fatto da chiunque, inclusi utenti e sviluppatori)
- La richiesta di cambiamento viene valutata rispetto agli obbietivi del progetto.
- Dopp la valutazione, il cambiamento viene accettato o respinto
- Se accettato, il cambiamento viene assegnato a uno sviluppatore e implementato.
- Il cambiamento implementato viene verificato

I progetti piccoli possono eseguire richieste di cambiamento in modo informale e veloce, mentre i progetti complessi richiedono moduli dettagliati di richiesta.

### Richiesta di Cambiamento 
Informazioni da documentare:<br>
- Nome/i e versione/i dell'Elemento/i di Configurazione in cui appare il problema
- Nome e indirizzo del richiedente
- Data della richiesta
- Indicazione di urgenza
- La neccessità del cambiamento
- Descrizione del cambiamento richiesto.

### Controllo dei Cambiamenti
Due tipi di controllo dei cambiamenti:
- <b>Promozione</b>:  lo stato di sviluppo interno di un software viene modificato
- <b>Rilascio</b>: un sistema software modificato viene reso visibile al di fuori dell'organizzazione di sviluppo.

Approcci per il controllo dei cambiamenti:
- Approccio informale
- Approccio formale

### Directory SCM
<b>Directory del Programmatore:</b>

- Libreria per contenere entità software appena create o modificate.
- L'area di lavoro del programmatore è controllata solo dal programmatore
<b>Directory Master:</b>

- Directory centrale per tutte le promozioni
- Gestisce la/le baseline corrente/i e controlla le modifiche apportate ad esse.
- L'ingresso è controllato, di solito dopo verifica
- Le modifiche devono essere autorizzate.

<b>Repository del Software:</b>

- Archivio per varie baseline rilasciate per uso generale
- Copie di queste baseline possono essere rese disponibili alle organizzazioni che ne fanno richiesta.

### Policy di Cambiamento
Ogni volta che viene eseguita una promozione o un rilascio, si applica una o più policy.<br>
Lo scopo delle policy di cambiamento è garantire che ogni versione,revisione o rilascio sia conforme a criteri comunemente accettati.<br>Esempi di policy di cambiamento:
- Nessuno sviluppatore è autorizzato a promuovere codice sorgente che non può essere compilato senza errori e avvisi
- Nessuna baseline può essere approvata senza essere testata da alemno 500 persone esterne.

### Ruoli tipici della Gestione della Configurazione

<b>Configuration Manager: </b>

- Responsabile dell'identificazione degli elementi di configurazione
- Può anche essere responsabile della definizione delle procedure per la creazione di promozioni e rilasci.

<b> Membro del Comitato di Controllo dei cambiamenti</b>

- Responsabile dell'approvazione o del rifiuto delle richieste di cambiamento.

<b>Sviluppatore</b>

-  Crea promozioni innescate da richieste di cambiamento o dalle normali attività di sviluppo
- Registra i cambiamenti e risolve i conflitti.

<b>Verificatore (Auditor)</b>

- Responsabile della selezione e valutazione delle promozioni per il rilascio e per garantire la coerenza e la completezza di tale rilascio.

### Audit e Revisioni della Configurazione
Un <b>audit</b> determina per ogni Elemento di Configurazione se possiede le caratteristiche fisiche e funzionali richieste.<br>Una <b>revisione</b> è uno strumento di gestione per stabilire una baseline.<br>Per ogni audit o revisione è necessario definire:
- Obbiettivo
- Elementi di configurazione in revisione
- Il programma per la revisione
- Procedura per lo svolgimento della revisione
- Partecipanti per qualifica professsionale
- Documentazione richiesta
- Procedura per la registrazione delle carenze e come corregerle
- Criteri di approvazione

### Gestione dei Branch

Mentre il software viene rilasciato in modo sequenziale,lo sviluppo di diverse funzionalità può essere eseguito da team diversi in modo concorrente e succesivamente unito in una singola versione.<br>Un <b>branch</b> identifica un percorso di sviluppo concorrente che richiede una gestione della configurazione indipendente.<br>La sequenza di versioni creata da ciascun team è un branch, che è indipendente dalle verioni create dagli altri team.<br>Un branch è identificato dal numero di versione da cui è stato derivato, seguito da un numero univoco.

### Gestione delle Varianti
Le varianti sono versioni che sono destinate a coesistere.
- Esempi: variante per diverse piattaforme,varianti di rilascio con più livelli di funzionalità
Esistono due approcci per gestire le varianti:
- <b>Team ridondanti:</b>
    - Un team è assegnato a ciascuna variante
    - A ciascun team vengono forniti gli stessi requisiti ed è responsabile della progettazione,implementazione e test delle varianti.
    - Un piccolo numero di elementi di configurazione è condiviso tra le varianti
- <b> Progetto Singolo: </b>
    - Progettare una scomposizione in sottoinsiemi che massimizzi la quntità di codice condiviso tra le varianti.
 
 ### Strumenti per la gestione della Configurazione del Software

 La gestione della configurazione del software è normalmente supportata da strumenti con diverse funzionalità, come:

- RCS - 1982:

    - Molto vecchio ma ancora in uso; solo sistema di controllo della versione.

- CVS (Concurrent Versions System) - 1986:

    -  Basato su RCS, consente il lavoro concorrente senza blocco (locking).

- SVN (Subversion) - 2000:

    - Sviluppato da Apache Software Foundation, con l'obiettivo di essere un successore per lo più compatibile di CVS.

- git - 2005:

    - Sistema di controllo della versione distribuito creato per lo sviluppo del kernel Linux. Piattaforme come GitHub, GitLab e Gitea sono basate su git.

- Perforce:

    - Server di Repository; tiene traccia delle attività dello sviluppatore.

- ClearCase:

    - Server multipli, modellazione dei processi, meccanismi di controllo delle policy.




