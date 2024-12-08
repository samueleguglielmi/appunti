Durante la generazione del file eseguibile di un programma, il compilatore ed il [[Linker]], generano all’interno del programma dei collegamenti tra istruzioni e [[Indirizzi relativi]] (indirizzi logici), mentre all’atto del caricamento questi indirizzi vengono trasformati in [[Indirizzi assoluti]] (indirizzi fisici).

Un codice con tali caratteristiche si chiama codice rilocabile.

La rilocazione è lo spostamento di un [[Processo]] in memoria.

In seguito ad una operazione di swap out la posizione di un processo, quando ritorna in [[RAM]] può non essere la stessa. È necessario modificare il codice.

Es. 
`indirizzo relativo nel program counter (500. 67h)`

`il programma subisce una rilocazione`

`il program counter ricalcola l'indirizzo tenendo l'offset uguale, ma la base diversa (300; 67h)`

