## Decidibilità e Indecibilità
Un problema di decisione è un problema detto decidibile se ha come soluzione si o no,
invece si tratta di un problema indecidibile se si tratta di problemi che sono irrisolvibili.


### Paradosso di Hilbert 1 - (Completo)
Nel paese senza confini esiste il più grande di tutti gli alberghi:
l’albergo con infinite stanze. Tuttavia anche gli ospiti sono infiniti,
e il proprietario ha esposto un cartello con la scritta *COMPLETO*.
Ad un tratto si presenta un viaggiatore che ha assolutamente
bisogno di una camera per la notte. Egli non fa questione di prezzo
e infine convince l’albergatore, il quale trova il modo di alloggiarlo.
Come fa?
Sposta tutti i clienti nella camera successiva (l’ospite della 1 alla 2,
quello della 2 alla 3, etc.); in questo modo, è possibile, essendo
l’albergo infinito, sistemare (nella camera 1) il nuovo ospite anche
se l’albergo è pieno.

### Paradosso di Hilbert 2 - (Comitiva Turisti Dispari)
Poco dopo arriva una comitiva di infiniti turisti, anche in questo
caso l’albergatore si lascia convincere, in fondo si tratta di un
grosso affare, e trova posto ai nuovi infiniti ospiti con la stessa
facilità con cui aveva alloggiato l’ospite in più
Come fa, senza ripetere infinite volte il passo visto prima?
Sposta ogni ospite nella stanza con numero doppio rispetto a
quello attuale (dalla 1 alla 2, dalla 2 alla 4,etc.), lasciando ai nuovi
ospiti tutte le camere con i numeri dispari, che sono essi stessi
infiniti, risolvendo dunque il problema. Gli ospiti sono tutti dunque
sistemati, benchè l’albergo fosse pieno.

### Paradosso di Hilbert 3 - (infiniti Alberghi)
Ancora più difficile: ci sono infiniti alberghi con infinite stanze tutti
al completo. Tutti gli alberghi chiudono, tranne uno. Tutti gli
ospiti vogliono alloggiare nell’unico albergo rimasto aperto.
Come fa (senza ripetere infinite volte il passo visto prima)?
Assegna ad ogni persona una coppia di numeri (n, m) in cui n
indica l’albergo di provenienza, e m la relativa stanza. Gli ospiti
sono quindi etichettati in questo modo:

(1, 1) (1, 2) (1, 3) (1, 4)... <br>
(2, 1) (2, 2) (2, 3) (2, 4)... <br>
(3, 1) (3, 2) (3, 3) (3, 4)... <br>
...  .. . . .. . ............. <br>

Adesso assegna le nuove stanze, per diagonali: <br>
1       --> (1, 1), equivale alla prima diagonale <br>
2, 3    --> (1, 2), (2, 1), equivale alla seconda diagonale <br>
4, 5, 6 --> (1, 3), (2, 2), (3, 1) <br>
e cosi via... <br>

Il problema si crea quando si cerca di confrontare 2 o piu insiemi infiniti, per determinare quale dei due sia piu grande: aaaaa
