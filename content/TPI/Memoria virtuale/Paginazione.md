Obiettivi:
● Mantenere in memoria solo le parti necessarie

● Gestire ogni volta solo piccole porzioni di memoria

● Non sprecare spazio evitando la frammentazione

● Poter usare porzioni di memoria non contigue per lo stesso
programma

● Non dare l’incombenza della suddivione del programma al
programmatore

La memoria fisica viene suddivisa in blocchi di dimensione fissa detti frame o pagine fisiche.

Il [[Programma]] è suddiviso in blocchi di uguale dimensione detti pagine o pagine logiche.

Se il numero di pagine logiche è minore del numero di pagine fisiche il programma potrebbe
essere caricato tutto in [[RAM]]. Invece se le pagine logiche sono di più di quelle fisiche
il programma viene caricato parzialmente.

Per eseguire un programma, all’atto del caricamento iniziale, serve che nella memoria fisica venga caricata la prima pagina logica.

Il [[SO]] mantiene una tabella delle pagine dove il numero di frame è usato come indice della tabella.

Nella tabella sono memorizzate:
● indirizzi fisici iniziali di tutti i frame presenti nella [[RAM]]
● indicazione di pagina occupata / libera
● eventuale ID del processo caricato

Anche al processo è associata una tabella delle pagine, dove sono indicati quali segmenti di codice sono caricati in [[RAM]] e quali su disco. 

Tale informazione nella tabella è riportata attraverso l’uso di un bit, detto bit di validità, il cui valore è 1 se la pagina è in memoria, 0 altrimenti.

È l’[[MMU]] che provvede alla traduzione degli indirizzi da logici a fisici.
Per ottenere un indirizzo fisico si devono avere due elementi che vanno poi sommati insieme, ossia:

● numero di pagina fisica 
● spiazzamento nella pagina o offset 

Dal numero di pagina la [[MMU]] preleva dalla tabella delle pagine l’indirizzo fisico al quale deve essere sommato l’offset.

Nella fase di traduzione dall’indirizzo logico a quello fisico viene consultata la tabella
delle pagine e se il bit di validità è uguale a 0 si ha un [[Page fault]].