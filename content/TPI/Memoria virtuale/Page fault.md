Si verifica nel momento in cui, durante l’esecuzione di un programma viene fatto riferimento ad un’istruzione che non è presente in alcun frame.

Il [[SO]] deve allora provvedere al caricamento della pagina:

● se sono presenti in memoria frame liberi, la pagina viene caricata immediatamente

● se tutti i frame sono occupati, si deve scegliere un frame di pagina poco utilizzato, salvarne il contenuto su disco e caricare la nuova pagina nel frame appena liberato