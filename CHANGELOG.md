# Changelog

Tutte le novità di Energy Grid Tycoon, una versione per volta, dalla più recente.
Formato ispirato a [Keep a Changelog](https://keepachangelog.com/it-IT/1.1.0/); numeri di versione secondo il
[versionamento semantico](https://semver.org/lang/it/) (vedi la sezione «Versioni» del [README](README.md)).

Ogni versione ha queste sezioni, quando servono:
- **Novità**: cose nuove da provare;
- **Modifiche**: cose che funzionano diversamente da prima;
- **Correzioni**: errori sistemati;
- **Da sapere**: salvataggi non compatibili, problemi noti, avvertenze.

## [Non ancora pubblicata]

## [0.2.0-alpha.1] - 2026-11-14

Il gioco parla anche inglese. *The game now speaks English too.*

### Novità
- **Inglese**, oltre all'italiano. Nel menu iniziale e in quello di pausa la voce **«Lingua»** cambia lingua al
  volo, senza riavviare la partita.
- Al primo avvio il gioco usa la **lingua del sistema** (italiano su un computer in italiano, inglese altrimenti).
  La scelta fatta nel menu resta salvata.
- Nella versione web si può aprire direttamente una lingua aggiungendo `?lingua=en` o `?lingua=it` all'indirizzo.
- **Date e numeri** seguono la lingua: in inglese «18 Oct 2020», «1,500», «8.0 m/s».

### Modifiche
- Il pannello **«Casella»** è più alto: mostra fino a cinque righe di dettagli senza tagliarle.
- Nel menu iniziale la voce «Esci» è sempre l'ultima.
- Il suggerimento del pulsante ▶/❚❚ ora dice solo «tasto Spazio» (F cambia la velocità).

### Da sapere
- I salvataggi delle versioni precedenti si caricano.
- La traduzione inglese è nuova: se trovi una frase strana o sbagliata, segnalala.

### In English
- **English** is now available alongside Italian. Use **«Language»** in the start menu or the pause menu to switch
  at any time, without restarting.
- On first launch the game picks your **system language**; your choice in the menu is remembered.
- In the web version, add `?lingua=en` to the address to open it straight in English.
- Saves from earlier versions still load. The translation is new: please report anything that reads oddly.

## [0.1.0-alpha.2] - 2026-11-14

Menu, calendario e luce del giorno sulla mappa: il gioco ora ha un inizio, una pausa e un tempo che si legge.

### Novità
- **Menu iniziale** con il logo: Nuova partita, Continua (riprende l'ultimo salvataggio), Esci. Tutorial, livelli,
  sfide e mondo aperto sono segnati «in arrivo». In fondo la versione e il credito, con il link al sito
  dell'autore.
- **Menu di pausa** con **Esc**: Riprendi, Salva ed esci al menu, Nuova partita (con conferma). Il tempo si ferma
  finché il menu è aperto.
- **Calendario**: la partita comincia il **18 ottobre 2020**. In alto si leggono il giorno di gioco, la data e
  l'ora. Le stagioni seguono il calendario: si parte in autunno, l'inverno arriva il 21 dicembre.
- **Stagione nel pannello Meteo**, con la sua icona.
- **Giorno e notte sulla mappa**: la luce cambia con l'ora, e le nuvole scuriscono il cielo.
- **Schermo intero**: il gioco parte a schermo intero; **F11** passa alla finestra e viceversa.
- **Tablet e schermi touch** (versione web): un tocco è un clic, un **tocco lungo** è un clic destro.

### Modifiche
- Le linee elettriche fanno parte dei gruppi di costruzioni attaccate: un gruppo che tocca una linea collegata è
  collegato.
- Testi dell'interfaccia tutti in italiano (per esempio «Produzione dell'ultima ora»).
- L'equilibrio del gioco resta lo stesso: con le stagioni nuove una partita ben giocata si vince più o meno nello
  stesso tempo di prima.

### Da sapere
- I salvataggi della `0.1.0-alpha.1` si caricano: la data si ricava dalle ore già giocate.
- **Esc** annulla prima la costruzione scelta; se non c'è niente da annullare, apre il menu di pausa.
- Le versioni per Windows e macOS non sono ancora state provate su quei sistemi: se qualcosa non va, segnalalo.

## [0.1.0-alpha.1] - 2026-11-13

La prima versione da provare. Si gioca dall'inizio alla fine, ma è un'alpha: ogni segnalazione aiuta.

### Novità
- Mappa con colline, giacimenti di carbone e costa. Si costruiscono linee elettriche, miniere, centrali a carbone,
  pannelli solari, pale eoliche, batterie e quartieri.
- Giorno e notte, stagioni (giornate più corte e più nuvole d'inverno), meteo che cambia, con la previsione delle
  3 ore successive.
- Le costruzioni attaccate fra loro si collegano alla rete insieme: basta che una tocchi una linea o il municipio.
- Segnali sulle costruzioni: «non collegata» e «senza corrente».
- Riquadri informativi al passaggio del mouse su pulsanti, icone e costruzioni.
- Conferma prima di demolire, con lo stato della costruzione e il rimborso.
- Pulsanti per pausa e velocità (1×, 2×, 4×) con icone animate. Il grafico in basso mostra produzione, domanda ed
  energia nelle batterie.
- Obiettivi sempre visibili, schermata di vittoria o sconfitta, salvataggio manuale e automatico ogni giorno.
- Versioni per Windows, macOS e Linux, e una da giocare direttamente nel browser.

### Da sapere
- La partita parte in pausa: premi Spazio o ▶ per iniziare.
- Le versioni per Windows e macOS non sono ancora state provate su quei sistemi: se qualcosa non va, segnalalo.
- Il gioco non è firmato: al primo avvio Windows e macOS chiedono una conferma (vedi «Al primo avvio» nel README).
- In arrivo nelle prossime versioni: la luce del giorno e delle nuvole sulla mappa, lo schermo intero, il menu
  iniziale (arrivati nella `0.1.0-alpha.2`).
