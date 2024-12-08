
Creare note con Obsidian e pubblicarle su GitHub. Usiamo una [[VM Lubuntu]]

Prerequisiti:

Installare Obsidian: [https://obsidian.md/](https://obsidian.md/)

Installare NodeJS: https://nodejs.org/en/download/prebuilt-installer

Installare Git: https://git-scm.com/

controllo installazione NodeJS con il comando node -v

e controllo l’installazione dell’ NPV(node package manager) con il comando npm -v

Attenzione a non utilizzare la versione 23.0.0 di node js perché è ancora sperimentale

controllo versione Git (controllato nella Bash di Git)

comando: git --version

Utilizzo il comando: git clone https://github.com/jackyzha0/quartz.git su cmd.

  
Questo scarica una copia del repository Quartz (all'interno di una cartella chiamata quartz) e la archivia localmente sul tuo computer. Precisamente la directory quartz verrà creata nella stessa directory in cui si sta lavorando.

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXe_NuyM3qZhKxaEV2_-sf3rcy8V1ZU0kvR7r34_Ta0TSZjOFPjtS0Yz-85yOfcMRVq38XAyQDUiz08A0ZUibaZlWRqyJ-2UM7quog3PItolzY6bhbh2Y1c1rtCkH6mDDYPf1reepEAhIoFF9DK-LjN4u34?key=uUQtOtXgTpwj89WH-TNHVQ)

  

Installazione quartz

Entro nella directory quartz. Utilizzo NPM per installare le librerie necessarie

comando: cd quartz comando npm i

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdDAVns9ry_xm49ObgEydwT1oJ7dFWGtdOP-kyNiRJwq4I9b3jCuIS3oO0vcJJFjknlKVepUjvs_Nf0foCk6tJlPCNpBTD9VZ07NqISiLsW73M960pGSzVpm2LsfB7Cw_nnCGArQSYny-qXhUC4tRuKbUVn?key=uUQtOtXgTpwj89WH-TNHVQ)

Il messaggio ottenuto è un messaggio di errore, ovvero l’installazione è avvenuta, ma alcuni pacchetti sono configurati male, può darsi che sia la versione di npm.

Per sistemare gli errori utilizzare npm audit fix. L’output ottenuto indica che l’operazione si è svolta con successo.

Creazione progetto quartz

Usare il comando npx quartz create e selezionare la voce Empty Quartz.

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeZr6nL0VzNzcSF8xvg75tXp9FmBtTADxkv81TUtrRKNAkNioUHYb1GU_tZfZLyNnSRz73J4tc-W0Fnf2hS-M861-TcqHGknZ1S_hx2ztZZlqhpveIRyzsaMiBSz25-zA0EBp0sNXxTaz_tsyi47DAIejSG?key=uUQtOtXgTpwj89WH-TNHVQ)

Selezionare l’opzione: Treat links as shortest path (per le vault Obsidian)

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdd3xSniXOBErVkht1oI2vOXm-HbtY0xQB_Bfvp4H3ePV_uAbA_WarOKAD8-PspchEqiNoIbJeg1On7a2KujjPklnFPz-qiPsg9c_hFyc7sHEP40EAKpfRM2pPh190S-oTzF8GDElZHn2k0Pt-8kWcOVmxb?key=uUQtOtXgTpwj89WH-TNHVQ)

Creazione di una nuova repository su Github

Scegliere il nome e gli altri attributi. Verificare che l’opzione ADD a readme file non è selezionata.

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeljeYveAqaRq1Tc4Ld-_TjY6M9LUU0-GMdooBr-o_Duwy4orOXi_4iojQh1Wgb68glCs6A6aQQjc-yboRcmpNxbJthSW8y8P95osZ3hbofRT83CfzDyb8XLqaNaXpLhT4c4q_B3acM013p2HtIT9spf3BR?key=uUQtOtXgTpwj89WH-TNHVQ)

  
Copiare il link ottenuto

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdTVRVBKvagpUpBVl8oUNT2QySTGGia6wzTHR06x6unI5qNTSZxkgK8txE680zZrHukAIOWPSCx_j45qzrfWRjUyGq0xyPJoVa-szuTSS8Qplaxx9ZjyzoSQuZ8Fgd1uBn0cjQadHa1bX3X15erjh2HysLt?key=uUQtOtXgTpwj89WH-TNHVQ)

Nel terminale eseguire il comando git remote -v. Mostra due remoti, origin e upstream, ognuno dei quali ha un fetch e un push.

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcbC3Vqd2JOKXYuYHp5-awAupjPz1AE-CODG3N0NGEd5_sMAbxhAzCP7ShnePAo3QTDChn3UcEWowwHgFIN3AbaylhkCgk6NNXViEnVy_dvjmXh95bTlD4ouuBI0x-15ZZncPSo91AQnn4_cH2jR4xJhZ1m?key=uUQtOtXgTpwj89WH-TNHVQ)

Eseguire il comando git remote rm origin. Rimuove le remote origini.

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfLbu37i6HkHNipfm2qv0x3piapP0YGY7Zw0jtoYuSTtinXe-bJj8biyOmW5ttiT0Q2fteazhIyV9H3ZWA47-Y8C0lhGST3_jFAcPJSQcw1FvwHjjx1rtIBAUfl7xoKupPmXk7C_QSCjvcKXH_90vTEL6I?key=uUQtOtXgTpwj89WH-TNHVQ)

Aggiungere le remote con il comando git remote add origin [link ottenuto su GitHub] 

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcMeM7mTK0GgsB9NUYTleUgQzpTiehjZO7emeV9PHi7FEP8eFi98txtE7WF43f0BbdLQH-0Cmc1md0gQ1eSmmoFcFYE-XDvq1S9__eIizPq6fqy_ToQfIzpcDuWHXK0BX3kBwAbY--g6_6v-DZnDLN8l58c?key=uUQtOtXgTpwj89WH-TNHVQ)

Controllo delle remote

comando: git remote -v

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeBaQ4TaWzvRQ0PTCl5V_DNJYtxleEmqzuACrehuALpo-FsU4N_yfhi2tugSx4PjdurCYvnSL_6RrSB4qzz_xSYyKjIPw9r4Hw9-jVMA9HD6Blb5J-D7U1oCJH9G55xlWFYeinaoz9HwAD6JoCq5fBR0oCv?key=uUQtOtXgTpwj89WH-TNHVQ)

Sincronizzare i cambiamenti

L'obiettivo è fare in modo che le modifiche fatte nella repository locale my-notes vengano apportate nella repository remota su GitHub.

comando: npx quartz sync --no-pull

Se è la prima volta che lavorate con GitHub vi verrà chiesto di accettare l’ecosistema Git. 

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXduMKsSzGffwLgu6hAZRqFRzPFGdefiSZX1ltfp_WV3zIEvIEsz2w0RXVw_MFQ-OVq1hthYQA9nD1DScGxY49CX6iohdiueJJEVjHQ-edtY73R94ZMGlgOjdvyTLIuSyR7PrQtI1pI2G62dotEx6vj0vWsE?key=uUQtOtXgTpwj89WH-TNHVQ)

L’icona chiederà all’utente di approvare che le modifiche effettuate online vengano fatte anche sul dispositivo utente e viceversa. È necessario per continuare con la procedura.

Una volta completata l’operazione, questa verrà segnalata dalla scritta “Done!” ![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXf7X6levf8Wb3g7Hn1V7cXOEqlcPTr1O-qVOzdXLE6KA-cM9gaLu_4BQ8p1gpaPYJCV44UYXj7Z7E56ouIMG9eUWu4yeaXciGMOS7kxUIAXlJUP3iye5H82n0GwR18wLMY0iPlqWhq-GcFm_dv6c-Si0UOE?key=uUQtOtXgTpwj89WH-TNHVQ)

In questo comando possiamo notare che da l’ errore:

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfEE9ugHYILipjonoLdUoIKbPUPV-9-RiE7DBiAasZAQ_LLgE5EGIj6LukBfDbSQovaJLtbp_jJnqBGINvlzmqKg1cF0yeJdqxYiHtKF0Thv5l-1frHGluO3K_9jhC7mkg1xa33_T63URka2TLedetyRCF4?key=uUQtOtXgTpwj89WH-TNHVQ)

L’errore viene perché non sono state date a Git l’email dell’account e la directory del dispositivo. Come ci viene specificato nel terminal bisogna usare i comandi:

git config user.name

git config user.email

Questi comandi dicono a git quale directory deve collegare e con quale email.

Dopo averli definiti, ripetere il comando  npx quartz sync --no-pull

Le tue repository sono sincronizzate. D'ora in poi, ogni volta che esegui l'ultimo comando, tutte le modifiche apportate localmente verranno inviate alla tua repository GitHub.

Creare un Vault Obsidian

Avvia Obsidian e, quando ti viene chiesto quale deposito aprire, fai clic su Apri accanto a Apri cartella come deposito.

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfpsXJbC664FX6q9Ed24XQNoqDEMObPlas1TNSJR3Zw0044N8HpPTdiYLr7gaJR9QQevZNsZfH_UEJky3j2X6vkrdmk-1HT9mr6MUCJ_ougGDRBhFpj_fwk2GG81ree3iIuGOG0dlTPr_Tr9kKqeIehCpY9?key=uUQtOtXgTpwj89WH-TNHVQ)

Seleziona la cartella creata my-notes e clicca “Apri cartella”.

Ora si potrà modificare Obsidian come si vuole. Installare Templater per comodità.

Creare una nuova nota con Ctrl+n e ricopiare cosa c’è scritto nel sito.
  
![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcHc0MDY6U2bhiVvP3gLtkriJZkC_kSMWcWXy1JHOVbMYo-JRoBexX6vToI2g0OqDSa6D0-KlKyTSnlfxsmOhafIeTe4a3Yyaf9DdeGT9WAn2RLnJDxWWeS9xipz8gDz5sqPWyVuyCyBHh9tmTMTJ5dASLu?key=uUQtOtXgTpwj89WH-TNHVQ)  

Creare una cartella templates. 

Andare su impostazioni—Templater—Folder location.

Mettere il nuovo file nella cartella templates.

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeADUAfIxKu_9IembB3F6Zw6nCLlic_jBZ2DMQWLJS_xLOw0iK-4GINcFvL91YFxsHKIGKXhIDMJUZ2GcRqRGeVmr3mdWBvWr3Md_5s1DTX7Q22bpJrkSV5L-aZQejfn9gCspCvZy8AfEszASda8b3S7f6F?key=uUQtOtXgTpwj89WH-TNHVQ)

Collegare i file locali a GitHub

Prima di pubblicare le note online possiamo verificare che tutto funzioni localmente. Si usa il comando:

npx quartz build --serve

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeeJCLiik-Zt1RwhstjeM-Lm3kfQ8j-3pffUHByiQaQdRfQKd64ieGYWifEXKm9Xuq-NSGAd3xOb_pPzmRP1cVi3BSdommSYkXcU-pL5-FElF0eqZ_enGYbgKX92UHQiLVKkiW9b3kr5ip73DgFaRm3x5Yj?key=uUQtOtXgTpwj89WH-TNHVQ)

Se si vuole verificare che le modifiche fatte con Obsidian vengano eseguite in remoto si utilizza il comando:

npx quartz sync

L’ output indicherà se il comando è andato a buon fine. 

Per condividere le note fatte su obsidian bisogna creare un file deploy.yml. Questo può essere fatto usando il comando sul sito ufficiale di quartz, oppure tramite un editor basta creare un file nella directory .github—Workflows, estensione .yml

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdErIkyNXhIQwBb5AIaUquAc1VzbJYTXgQt7XxT1Yck6XDF-fhyZ9Rvx5QYYLsW7mj-iWaIHXUkKKMOhjYbQwIsjHH3jwE1ZGCB9TuKMHi2YIS1VI4eeX3WMjeDJ9hx24G407iRW2LJsgHYeA6L4OLRzv8?key=uUQtOtXgTpwj89WH-TNHVQ)

Su GitHub vado su settings—Pages(nella barra a lato). Sotto “Sources”, seleziono “GitHub Actions”. 

Per salvare i cambiamenti uso  npx quartz sync.

Il sito sarà disponibile <github-username>.github.io/<repository-name>.

Per visualizzare il sito senza errori è obbligatorio mantenere il file index.md; perché in sua assenza non si potrà vedere la documentazione pubblicata.