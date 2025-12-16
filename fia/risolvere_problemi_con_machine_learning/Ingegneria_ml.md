### Ingegneria del Machine Learning
Per progettare una soluzione di machine learning, dobbiamo pensare a un modello basato su data & software engineering.

**Modello CRISP-DM** = rappresenta il ciclio di vita di progetti basati su intelligenza artificiale e data science.

Cross-Industry Standard Process for Data Mining

Il **CRISP-DM** è un modello non sequenziale in cui le fasi diverse possono essere eseguite un numero illimitato di volte.

**Business Understanding** -> raccolta dei requisiti e degli obiettivi di business (che cosa deve fare il machine learner che stiamo progettando). Questa fase prevede la definizione dei cosiddetti obiettivi di business criteria, ovvero i criteri secondo i quali potremo accertare che il sistema è in linea con gli obiettivi di business.
Inoltre in questa fase bisona definire:
- la disponibilità delle risorse
- stimare i rischi
- definire i relativi piani di contingenza
- condurre analisi costi-benefici

**Output:** Da questa fase possiamo ricavare il **Piano di progetto**, documento che spiega l'esecuzione del progetto da un punto di visya di gestione **tecnica e socio-termica**

**Data Understanding** -> consiste nell’**identificazione, collezione e analisi** dei dataset che possono portare al raggiungimento degli obiettivi.

**Output:** Documento di analisi dei dati il quale riporta i metodi di estrazione ed analisi, e le relazioni tra i dati ed eventuali problemi di qualità 

**Data Preparation** -> In questa fase si preparano i dati in maniera tale da essere utilizzati nelle fasi successive del processo.

Questo include il feature engeneering la selezione delle caratteristiche del problema che hanno maggior potenza predittiva.

Questa fase include l'implementazione dei processi di pulizia dei dati, sulla base dei problemi di qualità riscontrati nella fase precedente.

Infine, i dati vengono formattati in una maniera tale che possano essere prese in input
da un modello di machine learning

**Output:** Insieme di dati di input, ovvero l’insieme di dati che verranno considerati in
fase di modellazione dell’algoritmo di machine learning.

**Data Modeling**

**Data Preparation**

**Data Preparation**

**Data Preparation**

**SCRUM** = modello che prende in considerazione dei blocchi di lavoro in sprint (brevi periodi di tempo). Prevede lo sviluppo incrimentale di ogni porzione del sistema.

Lo scrum prevede tre ruoli fondamentali:
- Il **product owner**, colui che rappresenta gli stakeholder (chiunque abbia interesse nel prodotto), definisce e prioritizza i requisiti
- Lo **SCRUM Master**, agevola il lavoro e coordina le attività di sviluppo (non ha nessuna responsabilità sulla gestione del personale)
- Il **team di sviluppo**, si occupano della documentazione e dello sviluppo del prodotto

Ogni sprint inizia con uno sprint planning, nel quale vengono definite le attività da compiere nel prossimo periodo temporale. Il lavoro è monitorato da riunioni quotidiane in cui vengono riportati i progressi che si chiamano scrum daily. Alla fine dello sprint viene effettuata una sprint review, dove il team mostra i progressi effettuati e poi viene chuso successivamente a una sprint retrospective, dove il team riflette suoi problemi riscontrati e definisci i miglioramenti da fare nel prossimo sprint.

**TDSP** = Team Data Science Progress nasce dalla compinazione di SCRUM e CRISP-DM, incorpora gli aspetti socio-tecnici nell'esecuzione dei progetti.

Le fasi sono simili al CRISP-DM solo che ne combina alcune:
- Il Business Understanding è uguale, nel quale vengono definiti gli obiettivi
- Combinazione delle fasi di data Understanding e la fase di data Preparation e si chiama **Data Acquisition & Understanding**
- Combinazione della fase di modelling e Evaluation, si chiama solamente **Modeling**
- Mentre poi c'è la fase di Deployment che è simile solo che ha a che fare con le scelte ingegneristiche per rendere un modello usabile.

La vera, grande differenza sta nel fatto che, ad intervalli regolari, viene
effettuata una fase di **customer acceptance**, ovvero una validazione di
come il sistema implementa i requisiti di business.
Inoltre, TDSP definisce sei ruoli espliciti:
- Solution architect: Progetta e manutiene le architetture delle applicazioni;
- Project manager: Il responsabile dell’intero progetto;
- Project lead: Simile allo SCRUM master, è il team leader
- Data engineer: Il responsabile della data acquisition;
- Data scientist: Il responsabile della data understanding;
- Application developer: Il responsabile dell’implementazione dell’applicazione;

