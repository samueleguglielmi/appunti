
Gli standard IEEE 802 LAN/MAN sono specifici per LAN Ethernet, LAN wireless (WLAN), reti wireless personali (WPAN) e altri tipi di reti locali e metropolitane. 

Il layer di collegamento dati LAN/MAN IEEE 802 è costituito dai seguenti due sublayer:

- **Logical Link Control (LLC)** - Questo sublayer IEEE 802.2 comunica tra il software di rete nei layer superiori e l'hardware del dispositivo nei layer inferiori. Agisce inserendo nel frame le informazioni che identificano il protocollo di livello rete utilizzato. Consentono a protocolli multipli di Layer 3 di utilizzare la stessa interfaccia e lo stesso supporto di rete.
-
- **Media Access Control (MAC)** - Implementa questo sublayer (IEEE 802.3, 802.11 o 802.15) nell'hardware. È responsabile dell'incapsulamento dei dati e del controllo dell'accesso ai media. Fornisce l'indirizzamento del layer di collegamento dati ed è integrato con varie tecnologie di layer fisico.

![[Pasted image 20241203194103.png]]

Il LLC rileva i dati del protocollo di rete e aggiunge informazioni di controllo del Layer 2 per favorire la consegna del pacchetto al nodo di destinazione. 

Il sublayer MAC controlla la NIC e l'altro hardware responsabile dell'invio e della ricezione dei dati sul supporto LAN/MAN cablato o wireless.

Il sublayer MAC fornisce l'incapsulamento dei dati:

- **Delimitazione del frame** - Il processo di framing fornisce delimitatori importanti utilizzati per identificare un gruppo di bit che costituisce un frame. Questi bit di delimitazione forniscono la sincronizzazione tra i nodi di trasmissione e quelli di ricezione.

- **Indirizzamento** - Fornisce l'indirizzamento di origine e destinazione per il trasporto del frame del [[Layer di collegamento]] tra dispositivi sullo stesso supporto condiviso.

- **Rilevamento degli errori** - Include un trailer utilizzato per rilevare gli errori di trasmissione.

Il Sublayer MAC fornisce anche il controllo dell'accesso multimediale, consentendo a più dispositivi di comunicare su un supporto condiviso (half-duplex).

Le comunicazioni full-duplex non richiedono il controllo degli accessi.