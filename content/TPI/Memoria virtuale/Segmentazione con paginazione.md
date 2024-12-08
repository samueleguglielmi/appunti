Questa tecnica ibrida di gestione della memoria prende il meglio delleprecedenti 

Paginazione:
– identificazione dei frame liberi attraverso i bit di validità
– scelta del frame libero, non necessariamente contiguo, in cui caricare una pagina, quindi senza alcuna frammentazione

Segmentazione:
– verifica degli accessi e delle operazioni
– condivisione di porzioni di memoria

La memoria centrale fisica è divisa in pagine fisiche (frame) di dimensione fissa.

Lo spazio di indirizzamento del processo è suddiviso in segmenti logici (segmenti) di dimensioni diverse, ciascuno suddiviso in pagine logiche.

I frame hanno la stessa dimensione delle pagine logiche; infatti vengonocaricate in essi.

L'indirizzo logico è costituito dalla tripla:

s (numero di segmento), p (numero di pagina), d (spiazzamento nella pagina)

L'indirizzo fisico è rappresentato come:
f (numero di frame), d (spiazzamento nel frame)

La [[MMU]] traduce l'indirizzo logico in fisico.