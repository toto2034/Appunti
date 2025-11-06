# CICLO DI VITA DEL SOFTWARE (CVS)

Software life cycle: inizia quando un prodotto softwere viene creato e termina quando non è più disponibile per l'uso.Comprende una fase di ideazione, di definizione dei requisiti, di progettazione, di implementazione, una fase di test, una di installazione e verifica e talvolta anche di ritiro.


Software development cycle: il periodo inizia con la decisione di sviluppare un prodotto software e termina cona la consegna del prodotto.Comprende una fase di definizione dei requisiti,una fase di progettazione, una di implementazione, una fase di test e una di installazione e verifica

## Modelli cicli di vita del Software

Un modello del ciclo di vita del software è una caraterizzazione descrittiva o prescrittiva di come un sistema viene o dovrebbe essere sviluppato

## Tipologie di CVS
Esistono vari modelli di  CVS, nati negli anni 50 e sono:

- Waterfall (Cascata)
- Prototyping
- Incremental delivery (approcci evolutivi)
- Spiral model

## Fasi di un CVS

Definizione: si occupe del cosa

Sviluppo: si occupa del come

Manutenzione: si occupa delle modifiche

## Modello a Cascata (WaterFall)

Popolare negli anni 70, esso di muove con un modello sequenziale lineare ovvero:
 - progressione sequenziale di fasi, senza ricicli al fine di controllare tempi e costi.
 
 - definisce e separa le varie fasi e attività del processo

Quindi ogni fase raccoglie un insieme di attività omogenee per metodi,tecnologie, skill del personale ecc.. , esse sono caratterizzate dalle attività (taks), dai prodotti di tali attività (deliverables), dai conrtolli relativi, e la fine di ogni fase è un punto rilevante del processo.
L'output di una fase sono input di una fase succesiva.

 <img src = "img/image.png" width=400 height=300 >

## Studio di fattibilità
Viene fatta una valutazione di costi e benefici e varia a seconda della relazione committente/produttore
### Obiettivo
- Stabilire se avviare il progetto, valutare le risorse umane e finanziarie necessarie
### Output -> Documento di fattibilità
- definizione preleminare del problema
- costi, tempi, modalità di sviluppo per ogni alternativa


## Analisi dei requisiti
Viene fatta un'analisi completa dei bisogni dell'utente e dominio del problema

### Obiettivo
- Descrivere le funzionilità e le caratteristiche di qualità  che l'applicazione deve soddisfare

### Output -> Documento di specifica dei requisiti
- manuale utente
- piano di acceptance test del sistema

## Progettazione
Viene definita una struttura opportuna per il SW, per poi scomporre il sistema in componenti e moduli, quindi si preoccupa del COME
### Output -> documento di specifica di progetto

## Fasi Basse Del Processo

### Programmazione e test di unità: 
Ogni modulo viene codificato nel linguaggio scelto
### Intergrazione e test di sistema
- composizione dei moduli nel sistema globale
- verifica del corretto funzionamento del sistema
### Deployament
Distribuzione e gestione del software presso l'utenza

### Manutenzione
Evoluzione del SW, seguendo le esigenze dell'utenza quindi comporta ulteriore sviluppo quindi racchiude in sè interazioni delle precedenti fasi

## Vantaggi e Svantaggi del modello a cascata

### Pro: 
-  ha definito molti concetti utili
- ha rappresentato un punto di partenza importante per lo studio dei processi SW
- facilmente comprensibile e applicabile

### Contro
- interazione con il committente solo all'inzio e alla fine
- il nuovo sistema software diventa installabile solo quando è totalmente finito.


## Altri cicli di vita
questi modelli derivano dalle critche fatte al modello a cascata:
- Variante del modello a cascata
- Modello trasformazionale
- Modelli con prototipo
- Modelli evolutivi ed incrementali
- Modelli basati su riuso
- Meta-modello a spirale


## Che cos'è la Protipazione
Un prototipo per aiutare a comprendere i requisiti o  per valutare la fattibilità di un approccio, grazie ad esso si riesce ad interagire con il committente per accertarsi di aver bene compreso le sue richieste specifiche. Dopo la fase d'uso del prototipo si passa alla produzione della versione definitiva del Sistema mediante un modello waterfall.
- mock-ups: Produzione completa dell'interfaccia utente

- breadboards: Implentazione di sottoinsiemi di funzionalità critiche del SS, non nel senso di fattibilità ma in quello dei vincoli pesanti posti nel funzionamento del SS (Carichi elevati,tempo di risposta, ...).

La Prototipazione può essere:
- "throw-away" : pervenire ad una migliore comprensione dei requisiti del prodotto da sviluppare
- "esplorativa" : pervenire ad un prodotto finale partendo da  una descrizione di massima lavorando a stretto contatto con il committente..
