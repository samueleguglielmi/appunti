
Installazione di una VM Lubuntu

Assicurarsi che sul dispositivo ci sia abbastanza memoria e che il processore sia basato su x64, per procedere con l’installazione.

Scaricare l’immagine dal sito ufficiale di lubuntu
Link: [https://lubuntu.me/downloads/](https://lubuntu.me/downloads/)

Requisiti minimi:

- 2 core
- 2GB di RAM
- 20GB di memoria di massa
  

Andare sotto la voce 24.04.1 LTS (Noble Numbat).

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdXUpWUr1h4OD1xW74mDRG9AoKM1Luvw53A4ROaDcGlr-V0H6MjZsV34LhficYiIvKZTgRyf6yASHEJGalFCH6G9sByDShNtYHUFtvFiRO7s8L2Fg3IykQmkt8WCrhXgA_ym5fFhx7huz-DfzQ5m8CUq8jo?key=uUQtOtXgTpwj89WH-TNHVQ)

Selezionare la voce Desktop 64-bit per scaricare il file iso.

Virtualbox

Creare una nuova VM con il file ISO si Windows 11.
Selezionare il file ISO ed il nome.

Indicare la RAM. Indicare le CPU

Quanto? 4GB+ Quante? 2core+

Abilitare EFI

Indicare la memoria di  massa 

Quanto? 64GB+

Per un’allocamento dinamico non selezionare l’opzione “Pre allocazione a dimensione intera”

Controllo  che l’immagine sia stata scaricata correttamente

Per verificare l’integrità uso il comando: 

sha256sum lubuntu-24.04.1-desktop-amd64.iso

Oppure 

Get-FileHash C:\percorso\lubuntu-24.04.1-desktop-amd64.iso -Algorithm SHA256 

Installazione

Attraverso il pulsante Avvio faccio partire la VM. Seleziono l’opzione “try to install lubuntu”. Ora apparirà l’interfaccia “prova o installa lubuntu”.

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXen_GSInXolb3ZXBW_Y5oBUGqNLn4znP46rMI7z0DUjjQUmBFektn1qnO_etjIzpfr3rtDqlirtRWdm_96BekGT7hZ-WvaFsnBmVSF77wMc8Hr5PhAlh1_0hUe3Ubty-CgohloeGAJ8QyfNF-c8gRrDIme4?key=uUQtOtXgTpwj89WH-TNHVQ)


Specifico le caratteristiche della macchina:

- Seleziono il luogo ed il fuso orario.


![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXexeI-KJqPQnVrsAyNsRFZYRgcfRcLDBJggf9hDwQAzH0rGtBsqdjls1yRjbRTAFVRKR2-N3jK-EEF0Zl6zh5IJ6qhJjhpoYFXdZ5-pZCgZ65w9rBCJiE5kx6MofSTteqlnXb0CfLG1LSPdOKKGQEhQ0KM?key=uUQtOtXgTpwj89WH-TNHVQ)

  

- Seleziono il layout della tastiera

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXch9SlLqls_MCsffp22Z7sjN4EhElIVArMqZRE3JT2npJU-olRq1r8SIrVl_SiF-Jc8rUNeEzPn6p9-NaiITtlYbc_IvcHNbV-J8RvwpDOfr6EeIychHu3WvJd3T_xNraOggA6eHUJ5GqrnVzpoBB5LUcdw?key=uUQtOtXgTpwj89WH-TNHVQ)

  
Selezionare l’opzione installare lubuntu. Ora bisogna selezionare la voce “installazione normale” ed aggiungo  i vari pacchetti di terze parti che mi possono servire.

  
![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXd9f7phs02oflYEXoUhufGQtRmPjVfMOoqLcJrCiqCUo8k2b74xuRRM4nRyPMwfHk5fhFet4ZoixEsWCq25WwDtmr2kKnQM-uQubFcsaNyBq7xW9uCs8zBPhAVPhnVcmPpimyzZrLyaMQpExWL7df0WpCuH?key=uUQtOtXgTpwj89WH-TNHVQ)  
  

Definire le partizioni

Ora ci sarà presentato con due scelte: Cancellare tutti i dati nel disco o partizionare manualmente il disco. 

Selezionare l’opzione cancella disco e lasciare le altre opzioni inalterate.

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdrlWLXGwShK3Jd-VDSOEvHQ9QPEwcj8tijnwYdmgD6z0aLMt03OqJM3_Miz6ttB1CYkRgFmkEqLqCir4u87HJ1ENcYplgVjRLDZ6fbak1LGkJBZ3so6Pu7rKNHfCXpbmjZiW5rZFhYj_Tj4Mt5SK8QwYyH?key=uUQtOtXgTpwj89WH-TNHVQ)

Setup utente

Creare l’utente definendo nome e password.

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXflbBgCaWHrJtRw0dzrkKQXBbDw9chr9O64bgOBWOiC9Ryb7TKTmz7FjwmbQksu4SiqaS66pjI5HKu4iYS9MW_E5hl6N7c_OjdjFaRunVun-QyMpgb3x1ydacAHGwf2g3IIrkb5bfEtblTlMliEErLDFCUY?key=uUQtOtXgTpwj89WH-TNHVQ)  

Infine, dopo aver controllato il riassunto, procedere con l'installazione. 

