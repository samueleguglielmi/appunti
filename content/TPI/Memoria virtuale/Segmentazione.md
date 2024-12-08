La memoria centrale fisica è divisa in segmenti fisici (frame) di dimensioni diverse, ognuno con un nome che lo individua (spesso un numero).

Lo spazio degli indirizzi di un [[Processo]] è diviso in segmenti logici (segmenti)
● un segmento è caricato in un frame di pari dimensione
● i segmenti di un processo possono essere caricati in frame non contigui, mentre quelli non
caricati sono conservati nell’area di swap (su disco)

La traduzione degli indirizzi logici in fisici avviene attraverso la tabella dei segmenti dove:
● il numero di segmento è usato come indice
● ogni voce contiene:
– l’indirizzo base di segmento (indirizzo fisico di partenza)
– limite del segmento (scostamento massimo nel segmento)

Segmentation fault: si verifica se un indirizzo fisico calcolato punta ad un segmento diverso dal
segmento in uso, ovvero lo scostamento massimo va ad invadere un segmento adiacente.

L'indirizzo logico è calcolato dal numero del segmento e dallo scostamento.

La [[MMU]] traduce l'indirizzo logico in fisico.

Vantaggi:
● La gestione di strutture dati dinamiche, che crescono e diminuiscono, è semplificata
● Viene facilitata la possibilità di condivisione di segmenti tra alcuni processi
● Si semplifica il [[Linking]] (creazioni di indirizzi logici) di procedure compilate separatamente
● Ogni segmento può avere un diverso tipo di protezione

Svantaggi:
● [[Frammentazione esterna]] della memoria nel caso in cui i segmenti vengano continuamente
caricati e scaricati in memoria
