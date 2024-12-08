Esempi di reti di accesso basate sulla contesa sono i seguenti:

- LAN wireless (usa CSMA/CA)
- LAN Ethernet di topologia bus legacy (utilizza CSMA/CD)
- LAN Ethernet legacy utilizzando un hub (utilizza CSMA/CD)

Queste reti operano in modalità half-duplex, il che significa che solo un dispositivo può inviare o ricevere alla volta. Pertanto, è necessario un processo specifico per stabilire quando un dispositivo può eseguire l'invio e cosa succede quando più dispositivi trasmettono dati contemporaneamente.

Se due dispositivi trasmettono contemporaneamente, si verifica una collisione. Per le LAN Ethernet legacy, entrambi i dispositivi rilevano la collisione sulla rete. 

Questa è la parte di rilevamento collisione (CD) di CSMA/CD.

La scheda NIC confronta i dati trasmessi con i dati ricevuti o riconoscendo che l'ampiezza del segnale è superiore al normale sul supporto.

In caso di collisione, i dati inviati da entrambi i dispositivi verranno danneggiati e dovranno essere ritrasmessi.