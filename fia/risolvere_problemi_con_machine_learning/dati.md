### I dati
L’intelligenza artificiale in particolare è una scienza che richiede un ampio utilizzo di dati.

**Ingegneria dei dati:** L’insieme delle tecniche e degli algoritmi che consentono l’estrazione, l’analisi e la preparazione di dati che siano fruibili da altre tecniche o algoritmi di data analytics.

Avere dati di qualità (che descrivono accuratezza, completezza e consistenza) è l’unico modo di costruire strumenti di intelligenza artificiale capaci di assistere gli utenti nel processo di decision making.

**Data governance:** Gestisce la disponibilità, usabilità, integrità e sicurezza dei dati. E’ basata su standard interni ad un organizzazione o politiche che ne regolano l’utilizzo.

**Data leakage:** è un Problema che si presenta quando un modello è capace di lavorare accuratamente in fase di addestramento, ma non in fase di rilascio.
**leaky predictor:** caratteristiche che ci aiutano a caratterizare il problema ma che nella pratica non saranno disponibili il più delle volte, portando al fallimento del modello.

**Dato** è un qualsiasi elemento di cui si dispone per formulare un giudizio o risolvere un problema

Ci sono tre tipi di dati:
- Dati Strutturati: righe e colonne sono ben definite, sappiamo esattamente per ogni colonna il significato di un dato (DATABASE, FILE XML, JSON)
- Dati Non Strutturati: sono dati più difficili da estratte poichè richiedono strumenti ad-hoc (MUSICA FOTO, VIDEO)
- Dati Semi-Struturati: sono a metà tra lo strutturato e non strutturato, la struttura non ha definizione stretta. I dati tabulati (tabelle), potrebberi avrìere dati mancanti o espressi tramite un formato non strutturato. Sono generalmente salvati come file.

## Data Preparation:
**Data Cleaning -> Feature scaling -> Feature selection -> Data balancing**

**Data Cleaning**: su tratta della pulizia dei dati, è utile quando abbiamo dati rumorosi o mancanti
Del Data Cleaning fa parte la fase **Data imputation**: Insieme di tecniche che aiutano a ridurre il problema dei dati mancanti. Quando ci ritroviamo dinanzi a dati mancanti nel dataset, possiamo semplicemente scartare le righe o le colonne, soluzioni non sempre applicabili, per questo motivo ci viene in aiuto l'imputazione statistica. L'imputazione statistica la quale si basa sull'applicazione di semplici tecniche statistiche per stimare il valore dei dati mancanti. (non può essere applicata su dati numerici, non considera l'incertezza).
Il data Imputation possiamo suddividerlo in: 
- Imputazione tramite most frequent imputation: i dati mancanti sono sostituiti dal valore più frequente contenuto in una colonna.
- Imputazione deduttiva: il progettista definisce una regola sulla base di una deduzione logica.

