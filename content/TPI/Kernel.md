E’ un insieme di programmi del [[SO]] che:

● permette l’interazione tra HW e SW
● è l’unico autorizzato ad accedere direttamente all’hardware,
● gestisce le risorse HW nel modo più efficiente possibile
controllandone tutti gli accessi
● è responsabile dei driver più importanti
● è responsabile per la trasmissione e la mediazione dei comandi.

Quando n programma utente invia [[System call]] (“chiamate di sistema”) al kernel. Questa chiamata di sistema viene tradotta dal kernel in una serie di comandi inoltrati alla [[CPU]].

Funzioni:

Gestisce la memoria: controlla quanta RAM viene
usata e dove.

Gestisce i processi: determina quali processi possono usare la CPU,
quando e per quanto tempo.

Interagisce coi Driver del dispositivo: si occupa dell’intermediazione tra
l’hardware e i processi.

Gestisce chiamate di sistema: accetta richieste di servizio dai processi.

Per fare in modi di accedere ai servizi del Kernel è necessaria una [[Shell]].