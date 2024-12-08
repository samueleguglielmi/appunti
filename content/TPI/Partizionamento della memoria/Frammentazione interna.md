Si verifica quando un job è abbastanza piccolo da essere contenuto in ogni partizione ma, le partizioni sufficientemente grandi da contenerlo hanno la coda piena, mentre la coda di una partizione più grande è vuota, il job verrebbe assegnato ad una partizione grande determinando così uno spreco di memoria.

Si fa uso di una singola coda di ingresso. 

Strategie da adottare:

● si percorre la coda dall’inizio fino a individuare un job che possa essere contenuto nella
partizione libera

● si percorre tutta la coda individuando il più grande job che possa essere contenuto nella
partizione libera. Inconveniente: i job più piccoli rischiano di essere discriminati.