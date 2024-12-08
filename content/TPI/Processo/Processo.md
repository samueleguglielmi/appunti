Un processo o task è un' istanza di programma in evoluzione, cioè che è eseguito dal processore, quindi deve risiedere in [[RAM]] (entità dinamica)

Un processo è un [[Programma]] in esecuzione. 
Le funzioni di un processo sono chiamate threat o sottoprocesso.

L’esecuzione di un processo è formata da un alternarsi di fasi di uso della [[CPU]] a fasi di attesa di esecuzione di operazioni su altre risorse di sistema).

Ogni processo è costituito da:

- codice (composto dalle istruzioni);

- dati del programma, a loro volta suddivisi in:
– variabili globali, allocate nella [[RAM]] nell’area dati globali
– variabili locali e non locali memorizzate in uno stack
– variabili temporanee introdotte dal compilatore (tra cui PC o IP)caricate nei registri del processore
– variabili allocate dinamicamente durante l’esecuzione, memorizzate in un heap

- [[PCB]]

L’insieme di tutti i dati di un processo prende il nome di contesto del processo

I processi possono essere:

● Indipendenti: un processo può evolvere autonomamente senza necessità di
scambiare dati con altri processi

● Cooperanti: due o più processi per evolvere necessitano di scambiarsi informazioni

● Competitori: due processi possono ostacolarsi a vicenda, per usare la medesima
risorsa

