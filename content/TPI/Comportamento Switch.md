Uno switch Ethernet di Layer 2 utilizza indirizzi MAC di Layer 2 per prendere decisioni di inoltro. È completamente ignaro dei dati trasportati nella porzione dati del frame. Lo switch prende decisioni di inoltro basate solo sugli indirizzi MAC Ethernet di Layer 2.

Esamina la propria tabella degli indirizzi MAC per prendere una decisione di inoltro per ciascun frame, a differenza degli hub Ethernet legacy che ripetono i bit su tutte le porte tranne la porta in ingresso.

Lo switch crea dinamicamente la tabella degli indirizzi MAC analizzando l'indirizzo MAC di origine dei frame ricevuti in una porta.  Lo switch inoltra i frame cercando una corrispondenza tra l'indirizzo MAC di destinazione nel frame e una voce nella tabella degli indirizzi MAC.
  
Ogni frame in entrata in uno switch viene analizzato alla ricerca di nuove informazioni da acquisire. Ciò viene fatto esaminando l'indirizzo MAC di origine del frame e il numero di porta in cui il frame è entrato nello switch.

 Se l'indirizzo MAC di origine non esiste, viene aggiunto alla tabella insieme al numero di porta di entrata. Se l'indirizzo MAC di origine è presente, lo switch aggiorna il timer di aggiornamento per tale voce. Per impostazione predefinita, la maggior parte degli switch Ethernet mantengono una voce nella tabella per 5 minuti.

Se l'indirizzo MAC di destinazione è un indirizzo unicast, lo switch cercherà una corrispondenza tra l'indirizzo MAC di destinazione del frame e una voce nella sua tabella degli indirizzi MAC. Se l'indirizzo MAC di destinazione è presente nella tabella, inoltra il frame sulla porta specificata. Se l'indirizzo MAC di destinazione non si trova nella tabella, lo switch inoltra il frame da tutte le porte ad eccezione della porta di entrata. Questa operazione è detta "unicast sconosciuto"

Quando uno switch riceve i frame da diversi dispositivi, è in grado di compilare la tabella degli indirizzi MAC analizzando l'indirizzo MAC di origine di ciascun frame. Quando la tabella degli indirizzi MAC dello switch contiene l'indirizzo MAC di destinazione, è in grado di filtrare il frame e inoltrare una singola porta.
