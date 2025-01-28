
## Comando Cat
  
Il comando cat, abbreviazione di concatenate, viene utilizzato per creare e visualizzare file di testo, nonché per combinare copie di file di testo.

Per visualizzare un file nell'output standard utilizzando il comando cat, digitare il comando seguito dal nome del file.

Il comando cat può essere utilizzato anche per reindirizzare il contenuto del file ad altri file o inserire un altro comando utilizzando i caratteri di reindirizzamento. 

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeBWGY2IE-f65NGYjGcHjfQ_53qfn4K6iGQoHsLFWsno2V1zCS-rPuuLPeXO29ylCnVW_eL4LxUNxkagwBGwMp-hSHKh_izGIo2etwGkuEdb4FhQFr4oX3tgQdHZs565XIz9gH2?key=bcDNBtDQ5aI82XJUlW-hbNZ5)

## Comando  >

Quando usi il simbolo > per reindirizzare stdout, il contenuto del file viene prima distrutto.

L'utilizzo di un simbolo di reindirizzamento sovrascrive un file esistente. Questo si chiama "clobbering".

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcdEnl-mu0VKzP1Iykzo_h1_BzG8BZDo5cQshE1OwYLpcRU1Elvl8oZQFtKcJrN5g--RwJ3iAZAcwCmQ94V49CvDKpnompk5GJX7oLsrb7yF00HYcxSGP0wxobpUSJt3ifPCEqzyg?key=bcDNBtDQ5aI82XJUlW-hbNZ5)

Puoi evitare di sovraccaricare un file usando >> invece di >. Usando >> aggiungi a un file.

Si noti che utilizzando >> tutti i dati esistenti vengono conservati e i nuovi dati vengono aggiunti alla fine del file.

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcXKUqKzHe1NGX1DaE-_z6JTp8AoTs7AukQjfGFAaaxcqLOxKN7zI71vR6V86JM09FZ2lqWQg47pTVIISS9oX0o1YEsf15QQsiNVrF8ei_UqibvPuLxvOk8XQUFW2-22YoKIkxa5Q?key=bcDNBtDQ5aI82XJUlW-hbNZ5)

Comando find, differenza tra stderr e stdout

Il comando trova consente la ricerca con una serie di opzioni come nome file, dimensione, data, tipo e autorizzazione.

Il comando find inizierà la ricerca nella directory specificata ed effettuerà la ricerca ricorsivamente in tutte le sottodirectory.

Attraverso l’esecuzione del comando  find~ -name "*bash*"  troviamo i file contenenti la parola bash. Utilizzando il comando find /etc -name host l’output sarà un errore perché non c’è il permesso.

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdZlWQbjft86GW3CwWgACmhMTRCmVDgO05Jo0-IqGOBZe3TWmSNoWs8-aInMqxdAVZdtu2gkOWCpkYMl8k7tMSCdBgnu846YTAUi71ntTSTvY91mUFQAp-h7xnmqaXH2u65COc_hQ?key=bcDNBtDQ5aI82XJUlW-hbNZ5)

Per reindirizzare l'output di errore in un file bisogna ricordare che il descrittore di stderr è il numero 2, quindi viene utilizzato insieme al simbolo > per reindirizzare l'output di stderr a un file chiamato err.txt. 

Nota che 1 > (descrittore relativo a stdout) è uguale a >.

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeKbLjx1hAknaNZKkoHEFV8S6KY492ENE9bOvKl20LkQPxYc6A6kZHOcN5YUx3q1jciKcOG66E0D9IgGlCC4uxNRaWn5uOK1i9c8pha8S8qhPjDIGtV_PqceA8JCidlxRykQ7HU?key=bcDNBtDQ5aI82XJUlW-hbNZ5)

Si può anche reindirizzare stdout e stderr in due file separati attraverso il comando find /etc -name hosts > std.out 2> std.err

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfx1ys2Y9bmwnkBS1vEEeExk_pEiNDlUcRhzejP-hi8YubYrMP5zvCVFIYgVfV6iZwBS_0HiYNB2g4XZrBgp0aupbJd3VFdIDIGsMPZx27ePtt6h9EU45cqmZi6UKOsjZSCnhyJ8g?key=bcDNBtDQ5aI82XJUlW-hbNZ5)

Per reindirizzare sia l'output standard (stdout) che l'errore standard (stderr) su un file, reindirizzare prima stdout su un file e quindi reindirizzare stderr sullo stesso file attraverso il comando find /etc -nome host > find.out 2>&1

La parte 2>&1 del comando significa inviare lo stderr (segnato dal 2) nello stesso file dove va lo stdout (segnato da 1)".

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXf-_q20NI5b1_q-W3z_6HrA6tK2xo1iHM_I5wLnNLuMHnQjOtexcH22wH1m0n85WUrUqG62HYsET3JXDYl0N3JrcXzy5ctt56CTqZdBCbi2FxKi5Whgd_P-tTIuczGNQ2YAhAT04g?key=bcDNBtDQ5aI82XJUlW-hbNZ5)

Anche l'input standard (stdin) può essere reindirizzato. Normalmente stdin viene dalla tastiera, ma a volte può provenire da un file. Il comando tr traduce i caratteri, ma accetta solo dati da stdin, mai da un nome di file fornito come argomento. 

Il comando tr accetta l'input da tastiera (stdin), traduce i caratteri e quindi reindirizza l'output su stdout  

Si può quindi immettere dati da tastiera attraverso il comando tr a-z A-Z, i quali verranno tradotti in maiuscolo. Per uscire uso Ctrl+d. 

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcLHHoXpCvgnHfPw-Se6bMETFx-WqlqB3pSBQpoxntsQ3XIrZYO31QIMT0kMuoGt6Ihn-uCOHdrhA_851t-Fq36LrsXXzZIzIUI0v6eGNJVFJIOkpeFd5uzE43QlY2B5Kj22AjYhg?key=bcDNBtDQ5aI82XJUlW-hbNZ5)

Si può quindi trasferire i dati su un file ed eseguire l’operazione opposta. Utilizzo il comando tr A-Z a-z > myfile

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfa_MqcULNS4LCAvom1bTq5PHagXeeuqtvGVT-qcGAjlnri33N3pUlZXPOJon3ewMDFoA-4YHq3HUEgDqb95vq8bOaeLuRTxXd_x9z9P477r_qMSsPyEbLNYGxHcLlgsmV0yHiKNw?key=bcDNBtDQ5aI82XJUlW-hbNZ5)

Oppure si può trasformare il contenuto di un file attraverso tr a-z A-Z < myfile

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcV9fmiTTsC4I90yJw8wnCSwnBziQQh_3CK3l_NPsRShMR-C-SqggUuxtRQ3ulA2gEs6NmNKaXIdY7ObTWdWrfqppUXXUxjJQnMtpbsYNrLfwMKMECljCdct0GZ02IaWYxbJvh0WQ?key=bcDNBtDQ5aI82XJUlW-hbNZ5)

Ridimensionare l’output con more, less, cut, sort

Un'altra forma popolare di reindirizzamento consiste nel prendere l'output di un comando e inviarlo a un altro comando come input. Ad esempio, l'output di alcuni comandi può essere massiccio, si può quindi prendere l'output del comando ls e inviarlo al comando more attraverso il comando ls -l /etc | more.

Il comando cut è utile per estrarre campi da file che sono delimitati da un carattere, come i due punti: in /etc/passwd, o che hanno una larghezza fissa. Ad esempio possiamo estrarre tutti gli username dal file /etc/passwd attraverso il comando cut -d: -f1 /etc/passwd

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXf_2A_kXAAX7As5eQ3YXfjhMcjpawsBa45-EvEINurLThJqNVZR2oRIOohppndecZlDTPTd24A4LmtbAvP2j3T5VP-Z2JpYj7_YVNE3Mx7o2sjPGf5E83mTiTW7paEB4t1ABju7Kw?key=bcDNBtDQ5aI82XJUlW-hbNZ5)

Si può ordinare l’output attraverso la parola “sort”. 

Esempio: cut -d: -f1 /etc/passwd | sort. 

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeted7467jiHwUBCV36tsFDGq4vSEp8TZWyC0RSwUUxQjpP-fenC00A2ziwRnRe8jRYfrj1NuL38BzmYTKeh0IC_7bh-MO1dRF1-orSsMlb_jkWItNpX73RM88zcmyZ2ik_b1OaTA?key=bcDNBtDQ5aI82XJUlW-hbNZ5)

Per evitare che l’output sia troppo lungo basta aggiungere “more”. 

Esempio: cut -d: -f1 /etc/passwd | sort | more

Vedere file di larghe dimensione e relativi comandi e opzioni

Attraverso cat è possibile vedere il contenuto per intero di un file di grandi dimensioni come /etc/passwd.

Eseguire cat /etc/passwd

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdbgVfyoRCs168wpuqiUNxHETcyeHc-5bpaTVjV22RavUqw9WNiL7bDmFgG_ZmNgEIeoVF8q4KSesdVL_bv4lvPY3TZdQqexI80VYaCWGWyQZrfxVxkGqVn4skReGL-cz3roSXpIg?key=bcDNBtDQ5aI82XJUlW-hbNZ5)

Attraverso il comando more si ottiene la percentuale del file letto.

Comando more /etc/passwd

È possibile visualizzare il menu help schiacciando il tasto h

Attraverso il comando less /etc/passwd è possibile  cercare un termine specifico come bin.

Per muoversi avanti tra i risultati basta usare n, mentre N è ustata per muoversi indietro

È possibile utilizzare il comando head per visualizzare la parte superiore di un file. Per impostazione predefinita, il comando head visualizza le prime dieci righe del file.

Comando head /etc/passwd

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdZ6q63gjdGKN_4zsn_OxHesCoZ3auW95W_f_MCdUskEifzr_W0qxzmPCaKXdqBdKMWpwe9WN639HVbeMRhHm6pL9LdWFXM_Z2WA8V916NvInW3Xe5O4Fe7s_-tfFQmGVoRPDRVCg?key=bcDNBtDQ5aI82XJUlW-hbNZ5)

Utilizza il comando tail per visualizzare le ultime dieci righe del file.

Comando tail /etc/passwd.

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeEj6IEG8naJPCOJOLfBT_9iGe8YFYrAotMrFnH1x6pyt_PzF9-Umr5I6lAo3_1KeAWVvy5TP7crW7AgzQexTYLUEEJ-_EZvLjdtTdZtPxhVMCTQG0-y7x_EXijx-oeWW5W3k5wjA?key=bcDNBtDQ5aI82XJUlW-hbNZ5)

Possiamo specificare il numero di linee nell’output. Ad esempio si può stampare le prime 2 attraverso head -2 /etc/passwd.

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfbonee-phCUCziMzvwRSwwMJ4e7r2YDYkkbsL6-Fd7cGxLKxAv8bE3AIhvnCzyQIewTekr6TpLP0Z9K5cnFXFVN0Z32jUeybmA9JtC9xFlrULU49iyIXDmFPSeCCUcTscBEUsd4g?key=bcDNBtDQ5aI82XJUlW-hbNZ5)

Si può utilizzare il comando ls in combinazione con tail per visualizzare gli ultimi n nomi di una directory. Ad esempio /etc ls /etc | coda -5.

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXe6BCHIVsMAmIR8ZNnSCRagAS37pb9cSsHnZIDfgdkPvKsDQ_foQUJnCWSmQ8RL-nYSD7UGZpxQ6c6CivspvRKfv2fpgqlpi8P0EQTBawFFMdHsZC7EeIov2iUhug00KhaNcj6X0A?key=bcDNBtDQ5aI82XJUlW-hbNZ5)

Come hai visto, sia i comandi head che quelli tail producono dieci righe per impostazione predefinita. Potresti anche usare un'opzione -# (oppure puoi usare l'opzione -n ​​#, dove # è il numero di righe da visualizzare). 

Il comando head inizia a contare le righe in output dalla parte superiore dei dati, mentre il comando tail conta il numero di righe in output dalla parte inferiore dei dati. 

Un altro modo per specificare quante righe restituire con il comando head è utilizzare l'opzione -n ​​-#, dove # è il numero di righe contate dalla fine dell'output da escludere.Ad esempio, se /etc/passwd contiene 27 righe, il seguente comando visualizza le righe 1-7, escluse le ultime venti righe. Comando head -n -20 /etc/passwd

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfYF7hD08SjVmajlXpTDdECnBHVh7jZUmL_N20tweyjUS_4tjcxydRyZQdT17kysd2ipQR8aXcoRharDPykW6b19SK6Bt8trraoQb17GuOA6a3yj7Tf5xl-eBnz9Fo7R4IKNIyNtQ?key=bcDNBtDQ5aI82XJUlW-hbNZ5)

## Cercare testo attraverso espressioni

Il comando grep utilizza espressioni regolari di base, caratteri speciali come i caratteri jolly che corrispondono ai modelli nei dati. Il comando grep restituisce l'intera riga contenente il modello corrispondente.

L'opzione -E del comando grep può essere utilizzata per eseguire ricerche con espressioni regolari estese, essenzialmente espressioni regolari più potenti. Un altro modo per utilizzare le espressioni regolari estese è utilizzare il comando egrep.

Il comando fgrep viene utilizzato per trovare la corrispondenza con i caratteri letterali, ignorando il significato speciale dei caratteri delle espressioni regolari.

Il comando grep restituisce come risultato una data stringa di caratteri in un file come /etc/passwd. Comando grep sshd passwd.

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXe0Gxcd6v8M2YxQiZHN-Cj4zxoJ07pPIzKLalTkTLpxrd30pN_APvhZK-inhYn3a90JR6mUuIpOjN7xXxEMEE8-Y4Zk8gdYebDVjcgafsHj6oJzbxhbbprKRZy9sLStBtgPfNjF_g?key=bcDNBtDQ5aI82XJUlW-hbNZ5)

Restituisce il riscontro con tutti i casi in cui viene specificato il pattern. Ad esempio utilizzo il comando grep root passwd

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcVP88-b5oi0uD2OynBihEBPl47KQuJuV0-uDU5aJl8rPhQ_bt4luYTJdW8BOwYhz6SLWy_PSiOF3w5sH_-SRzJgG4WVMB3YgXKOgREJ0ZA64ul9FFZiSiUeLVXHMR6GA6NH_KoeA?key=bcDNBtDQ5aI82XJUlW-hbNZ5)

Per limitare l'output, puoi utilizzare le espressioni regolari per specificare. Ad esempio, il carattere ^ può essere utilizzato per trovare la corrispondenza con un modello all'inizio di una riga. Devono essere usati i singoli apici e non le virgolette.

Comando grep '^root' passwd

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeEOtkGeCyeFpb3sPXBe6EBpkmAcuOe47h65jzTmn5QP1wfWX77OCrHg9sCA6bLhjtnU7bQ0Z-H8N3TT0yfWys-2epiNJAJPEjsz5XNXdAOXsjt52Q54N6SQUafXMn3dDtYlqS_FQ?key=bcDNBtDQ5aI82XJUlW-hbNZ5)

È possibile trovare riscontro con “sync” ovunque su una linea

Comando grep 'sync' passwd

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdSAYe7b4xhTZsixqY9nHwbYcKgUr5dtmJD-N6lGrShWWWKBYlkEeHKTQ4FHihupF7rPCYM2sqh5dBRVll6reYfZtu-Qy7eIkdCFAGU8X65yI0pbYAWaP1dSAdJJvL920CrNAjYhA?key=bcDNBtDQ5aI82XJUlW-hbNZ5)

Utilizza il simbolo $ per abbinare la sincronizzazione del modello alla fine di una riga.

Comando grep 'sync$' passwd

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdPqBMH3S1OsLpsuIx8SU3SdYOQuWpTdtHWCS3V05NbWdt-jQnBt3y77l4AYghzLmxEpw86gthIouDPS8yOfoUfC9m3EKqoUSsuQxDfxPjDFy9NT4itRpW6iQDAWHs40xxFpa8o?key=bcDNBtDQ5aI82XJUlW-hbNZ5)

Utilizza il carattere . per corrispondere a qualsiasi singolo carattere. Ad esempio, i caratteri seguiti da una y.

Comando grep '.y' passwd

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeDJksT2hGEj7tR6cA9I_1C1gVw8t4NfpT_diZJ2lIKA4xOjC-neEP6E6k-GXBxPQHZllCb9p75LZSuLmetVlvW6lb-45rZMj-3hEMcY-sIhu79TqaB5Ehxzmbhu2HpnKPEz7CXvw?key=bcDNBtDQ5aI82XJUlW-hbNZ5)

Il carattere pipeline  | , funge da operatore "or". Ad esempio, esegue quanto segue per tentare di trovare la corrispondenza con sshd, root o operator:

Comando grep 'sshd|root|operator' passwd

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfadWSmnloWPmz1Hrs7_82y3vATJR5EBK03Z3MlumvQDC3HY2tw6lTNJSfqi9Ly7oRs690RqlNXskeDk_7yuwIqH4LP1MU1Plj51JEYeP9AmP0ZggGKcOJAnuHfR4vM6IQ_0-TAow?key=bcDNBtDQ5aI82XJUlW-hbNZ5)

Si noti che il comando grep non riconosce la pipeline come operatore “or”. Al comando grep bisogna aggiungere -E oppure usare egrep.

Utilizzare l'opzione -E per consentire a grep di operare in modalità estesa per riconoscere l'operatore di alternanza.

Comando grep -E 'sshd|root|operator' passwd

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcNoy1WYwR980kX8wlS4wrpUpQYB83ZwvbtVzfrH3Lxmp_uzduLAcytLD9yl4AaB0-Roa69voHoRmEi7chqDlfKm6WC_J_6mPBkZA1bgHwWDEhlRXNcap0ZsqO6V6_7RqLNDQun5g?key=bcDNBtDQ5aI82XJUlW-hbNZ5)

Possiamo usare egrep per trovare corrispondenze in un gruppo con pipeline. Ad esempio possiamo evidenziare le stringhe non e nob con il comando grep 'no(b|n)' passwd

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdxvu6h0WHQMnHpwt0Mp94acpqlWN5DerEJ8WH9squ8PvNQuECUqHdaQDztNVYlxmduOPyP0rpD_3fA6j2C7WGwabykAqkt7xjtFbwzWeAScEO8K1Gj2MU11yQ0uk9dmmMlrYv2Hw?key=bcDNBtDQ5aI82XJUlW-hbNZ5)

Le parentesi, ( ), venivano usate per limitare la "portata" del  carattere |. 

I caratteri [ ] possono essere utilizzati per trovare la corrispondenza con un singolo carattere. Tuttavia, a differenza del carattere punto, i caratteri [ ] vengono utilizzati per specificare esattamente quale carattere si desidera far corrispondere. Ad esempio un numero tra [0-9]. 

Comando head passwd | grep '[0-9]'

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXc78aDZ85zG6IpCBuh_yxS8A2i20GLHT1NWyaJ3YH5yZisTJaRnauuWvIseVm0gb4Q6rZ7e3ps9J_pEuc-KA_fWR892OnlyOaMWqg7PD-FjkgqL2djOAba_09xpD96ERTZU9A_kfA?key=bcDNBtDQ5aI82XJUlW-hbNZ5)

Il comando head è stato utilizzato per limitare l'output del comando grep.

Puoi utilizzare i caratteri { } contenenti un numero per esprimere che desideri ripetere uno schema un numero specifico di volte; ad esempio: {3}. 

Comando grep -E '[0-9]{3}' passwd

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdvwncLqkadhbjSlRyAXXa0p5NZZgz7eRk0WinXQZwa7U699_Pb_rjr2992OH8xt-_qEVrbegWcebMMibuX50QDVs_UD-WcfHUoCHMvwyXiDuxafKg9s-dRI_C9GHrjys4Nltau0w?key=bcDNBtDQ5aI82XJUlW-hbNZ5)
