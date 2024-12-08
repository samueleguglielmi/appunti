È la traduzione di un [[Programma]] da sorgente in codice macchina.

Il compilatore traduce il programma in moduli oggetto. Gli indirizzi di ogni modulo partono da 0. Ognuno ha dimensioni diverse.

Nei moduli vengono create tre parti:

- codice

- dati (variabili globali, ecc), ovvero lo spazio in memoria necessario per contenerli.

- riferimenti esterni

#### Riferimenti esterni

A causa delle compilazioni separate la traduzione del programma in codice non può essere effettuata completamente.

Quando è chiamata una funzione non è possibile specificarne l'indirizzo d'ingresso del salto, la cui destinazione, creata nel modulo main, è simbolica.
