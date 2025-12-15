### Agenti capaci di apprendere
L’apprendimento presenta il vantaggio di permettere agli agenti di operare in ambienti inizialmente sconosciuti diventando col tempo più competenti. 
L'apprendimento consiste in qualunque processo tramite il quale un sistema migliora le sue prestazioni sulla base dell’esperienza. 
Quindi l'apprendimento tecnicamente consiste nel migliorare l'esperienza di un task T rispetto alla misua di prestazione P, sulla base dell'esperienza E.

Un agente di questo tipo ha quattro componenti principali:
-> Elemento di apprendimento: responsabile del miglioramento interno.
-> Elemento esecutivo: responsabile della selezione delle azioni esterne. 
-> Elemento critico: responsabile di fornire feedback sulle prestazioni correnti dell'agente.
-> Generatore di problemi: responsabile di suggerire azioni che portino ad esperienze nuove e significative che portino l'agente ad apprendere nuove conoscenze da sfruttare poi per migliorare le sue azioni.

Machine Learning esplora lo studio e la costruzione di algoritmi che possano imparare dai dati e sulla base di questi fare previsioni. Questi algoritmi consentono di andare oltre alla programmazione classica perchè non si limiteranno a eseguire semplici comandi espliciti ma saranno in grado di prendere decisioni data-driven.

Possiamo distinguere l'apprendimento in supervisionato e non supervisionato:
-> quello supervisionato, è quando un agente apprende usando dei dati etichettati. Ogni dato input è associato a un output noto (etichetta data dal progettista dell'agente).
-> quello non supervisionato, è quello in cui un agente apprende usando dei dati non etichettati. L'agente sarà in grado di imparare senza conoscere il valore reale della variabile dipendente (etichetta), il progettista qui lascerà all'agente il compito di apprendere sulla base dei dati a disposizione.

Inoltre esistono altre tipologie di machine learning, cioè l'apprendimento semi-supervisionato e per rinforzo.
Nell'apprendimento semi-supervisionato alcuni dei dati sono etichettati altri no. L'agente intelligente sarà tenuto ad apprendere quali sono le etichette mancanti.
Invece nell'apprendimento per rinforzo, l'agente compierà azioni in maniera sequenziale e al termine di ogni sequenza, gli verrà assegnata una ricompensa che ha lo scopo di incoraggiare comportamenti corretti.

I problemi di machine learning si basa sull'output che i intende ottenere:
Per output si intende il range di valori che la variabile dipendente potrà assumere.
-> regressione: se è continuo;
-> classificazione: se l'output è discreto si paral di classificazione;
-> clustering: quando c'è suddivisione dei dati in gruppi.
-> Riduzione della dimensionalità: usata per ridurre le caratteristiche significative ed eliminare le caratteristiche ridondanti
-> Mining di associazioni: serve ad identificare dei pattern comuni in un insieme di transazioni. 

Quindi qual'è algoritmo migliore? Ci si basa sul metodo empirico, cioè grazie alla teoria si fa una selezione degli algoritmi che possono essere utilizzati per quella tipologia di problema e poi grazie alla pratica scegliamo la soluzione migliore. Per la pratica utiliziamo la misura di errore che ci permette di testare gli algoritmi scelti e utilizzare quelli con i risultati migliori. Quindi la misura di errore ci fornisce una base di confronto tra più modelli.

Errore. L'errore, o residuo, è la differenza tra il valore stimato della variabile da predire e il suo valore attuale.

Bias. Il modello ha un certo bias, se quando viene addestrato su diversi dataset, l'output che restituisce è sistematicamente sbagliato.

Varianza. Il modello ha una certa varianza se, quando viene addestrato su diversi dataset, l'output che restituisce è sistematicamente diverso.

ERRORE= BIAS + VARIANZA <- Quindi l'obiettivo è rendere nulli bias e varianza.

Bias e Varianza sonoinversamente correlati -> tanto diminuisce il bias tanto aumenta la varianza e viceversa. Quindi è necessario trovare un compromesso bias-varianza, ovvero un compromesso tra la flessibilità del modello ed il comportamento su dati che non ha mai visto.

Problemi Underfitting e Overfitting

Underfitting -> Un modello con bassa precisione quando dovrà predire nuovi dati (sbaglierà molto frequentemento). Non potrà risolvere problemi complessi, ovvero i problemi per i quali i dati in input sono molto intricati. Tende a sotto-dimensionare i dati.

Overfitting -> Un modello con varianza elevato ètenderà a risolvere problemi semplici utilizzando soluzioni complesse, perchè non è capace di generalizzare le competenze acquisite sull'insieme dei dati in input. Tende a sovra-dimensionare i dati.

Underfitting e Overfitting, sono dei problemi da diagnosticare generati su un insieme di dati quanto più ampio possibile, più dati abbiamo, più è facile per un algoritmo di machine learning apprendere correttamente.

Alcune soluzioni tra underfitting e overfitting: 
- La selezione delle caratteristiche rilevanti , tramite la quale un algoritmo di machine
learning riesce ad apprendere “meglio”, focalizzando l’attenzione sui soli dati che
rappresentano la variabile dipendente;
- La convalida incrociata, tramite la quale vengono generate una serie di insiemi di dati
di test, così da consentire all’algoritmo di machine learning di perfezionare
l’apprendimento sui vari insiemi di test; 
- La configurazione dei parametri, quando possibile (per algoritmi parametrici). Questa consente di gestire meglio i dati di input e ridurre il rischio di overfitting e underfitting.
- L'aumento della dimensione dei dati di input






