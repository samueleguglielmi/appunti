Un [[Processo]] può trovarsi in una certa posizione rispetto alla [[CPU]].

I possibili stati sono:

●new: stato in cui si trova appena creato (quindi appena caricato in [[RAM]])

● ready: un processo è nello stato di pronto se ha tutte le risorse necessarie alla sua evoluzione ad eccezione della [[CPU]]

● running: la [[CPU]] sta eseguendo le sue istruzioni, quindi a esso è assegnato il processore

● waiting: un processo è in attesa quando gli manca una risorsa per poter evolvere; quindi attende
che si verifichi un evento che lo riporti in stato di “ready”

● terminated: tutto il codice del processo è stato eseguito e quindi ha terminato l’esecuzione; il [[SO]]
può rilasciare tutte le risorse che utilizzava

Quando è creato un nuovo processo (caricato in [[RAM]] il programma), gli viene assegnato un identificatore ([[PID]]) e viene inserito nell’elenco dei processi pronti (RL, Ready List)

Quando gli viene assegnata la CPU, il processo passa nello stato di esecuzione,
dal quale può uscire per tre motivi:

– termina la sua esecuzione
– termina il suo tempo di CPU, cioè il quanto di tempo a sua disposizione, e quindi ritorna
nella lista dei processi pronti RL
– gli manca la disponibilità di una risorsa: per poter evolvere necessita di una risorsa al
momento non disponibile e quindi il processo si sospende e passa nello stato di attesa
formando la waiting list (WL). Dallo stato di sospeso un processo esce solo quando ottiene la risorsa, per passare poi nella RL dalla quale può essere prelevato per passare di
nuovo in stato di esecuzione.