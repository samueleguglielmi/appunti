Il layer di collegamento dati del modello ISO/OSI (Layer 2) prepara i dati di rete per la rete fisica. Il layer di collegamento dati è responsabile della scheda di interfaccia di rete (NIC) per le comunicazioni della scheda di interfaccia di rete. 

Il layer di collegamento dati esegue le seguenti operazioni:

- Consente ai layer superiori di accedere ai supporti. 
- Accetta i dati, di solito i pacchetti Layer 3 (cioè IPv4 o IPv6) e li incapsula in frame Layer 2.
- Controlla in che modo vengono collocati e ricevuti i dati sui supporti.
- Scambia fotogrammi tra endpoint attraverso il supporto di rete.
- Riceve i dati incapsulati, di solito i pacchetti di Layer3, e li indirizza al protocollo di layer superiore corretto.
- Esegue il rilevamento degli errori e rifiuta qualsiasi frame danneggiato.

Senza il layer di collegamento dati, i protocolli di livello rete, come il protocollo internet (IP), dovrebbero prevedere misure specifiche di collegamento per ogni tipo di supporto presente lungo il percorso di consegna. 
