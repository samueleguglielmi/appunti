All’atto dell’inizializzazione del sistema, staticamente viene stabilita la dimensione delle partizioni e viene creata una tabella che memorizza lo stato delle partizioni, indicando quali sono libere e quali occupate.

Le partizioni possono anche essere di dimensione diversa. Per ogni partizione viene gestita una coda dei processi in attesa in base alle loro dimensioni. In genere un nuovo job viene aggiunto alla coda della partizione più piccola che è in grado di contenerlo.

Soggetto a frammentazione interna