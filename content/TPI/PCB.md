Il [[SO]] per ogni processo deve mantenere delle informazioni, che tengano traccia di cosa sta “facendo il processo”. L’insieme di queste informazioni è
detto descrittore di processo (PCB, Process Control Block).
PD contiene:

● [[PID]] (Process Identifier)
● stato corrente
● Program Counter
● registri
● priorità
● puntatori alla memoria del processo
● puntatori alle risorse allocate al processo

Il PD è allocato dinamicamente alla creazione del processo, e viene rimosso dopo le
operazioni di teminazione del processo