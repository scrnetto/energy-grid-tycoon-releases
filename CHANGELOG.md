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

## [0.4.0-alpha.1] - 2026-11-15

La città ha fame: arriva il cibo. *The town gets hungry: food arrives.*

### Novità
- **Il cibo**: gli abitanti mangiano ogni ora. La scorta è nella barra in alto e diventa rossa quando sta per finire.
- **Quattro costruzioni nuove**:
  - **fattoria** (pianura): produce secondo la stagione, niente d'inverno;
  - **peschereccio** (costa): pesca tutto l'anno, ma si ferma col vento troppo forte;
  - **serra** (pianura o collina): produce tutto l'anno, ma consuma molta energia;
  - **magazzino frigorifero** (pianura): la città può tenere più cibo.
- **Il cibo passa dalla rete**: le costruzioni del cibo consumano energia. In un blackout non producono e i
  frigoriferi perdono una parte del cibo in più.
- **Importazione automatica**: se la scorta finisce il cibo arriva da fuori, a caro prezzo. Evita la fame ma non fa
  crescere la città, che per crescere ha bisogno di almeno un giorno di scorta propria. Senza soldi arriva la fame e
  gli abitanti se ne vanno.
- Nel pannello **Casella**: quanto cibo produce una costruzione, quanto spazio aggiunge un frigorifero e quanta
  energia consuma.
- **Luci di notte** anche su serre e frigoriferi.

### Modifiche
- I lavoratori vanno prima all'energia, **poi al cibo**, poi alle miniere, poi ai servizi dei quartieri.
- La disoccupazione pesa un po' di più sulla soddisfazione.
- Tasti da **1 a 9 e 0** per scegliere le costruzioni; il magazzino frigorifero si sceglie dalla lista.
- Lo stato del salvataggio è ora sopra il grafico dell'energia.

### Correzioni
- Con molte costruzioni nella lista la barra in alto e il grafico non vengono più schiacciati.

### Da sapere
- **Salvataggi in formato nuovo.** Quelli delle versioni precedenti si caricano: la città riparte con la scorta di
  cibo iniziale. I salvataggi della 0.4.0 non si aprono con le versioni precedenti.

### In English
- **Food**: residents eat every hour; the stock is in the top bar and turns red when it's low.
- **Four new buildings**: farm (nothing in winter), fishing boat (stops in strong wind), greenhouse (all year, uses
  a lot of power) and cold store (more storage).
- **Food runs on the grid**: food buildings use power, stop in a blackout, and cold stores lose some extra food.
- **Automatic imports** when the stock runs out: expensive, they prevent famine but the town only grows with at
  least a day of its own stock. With no money, famine hits and residents leave.
- Jobs now go to energy, then food, then mines, then services. Unemployment weighs a little more on happiness.
- Keys **1–9 and 0** pick buildings; the cold store is in the list.
- **New save format**: older saves still load with the starting food stock; 0.4.0 saves don't open in older
  versions.

## [0.3.0-alpha.1] - 2026-11-14

**Il gioco ha un nome nuovo: «Voltvale: Energy Grid Tycoon».** *The game has a new name: «Voltvale: Energy Grid Tycoon».*

### Novità
- **Nome e logo nuovi**: Voltvale. «Energy Grid Tycoon» resta come sottotitolo.
- **Tre lingue in più**: tedesco, francese e spagnolo, oltre a italiano e inglese. Al primo avvio il gioco usa la
  lingua del sistema, se è una delle cinque.
- **Il lavoro**: circa il 56 % degli abitanti lavora. Centrali, impianti solari ed eolici e miniere hanno bisogno di
  personale: con poco personale producono meno, senza si fermano (segnale del casco barrato). I lavoratori vanno
  prima all'energia, poi alle miniere, poi ai servizi dei quartieri. La disoccupazione abbassa le tasse e un po' la
  soddisfazione. Nella barra in alto: occupati / forza lavoro; nella casella di ogni edificio: «Personale».
- **Luci di notte**: le finestre di quartieri e municipio si accendono al tramonto e si spengono se manca corrente.

### Modifiche
- La scritta «(in pausa)» compare solo quando il gioco è davvero in pausa.
- A partita iniziata l'avviso di pausa dice «per riprendere».
- Nelle lingue con parole lunghe la barra in alto e il pulsante «Demolisci» non escono più dallo spazio.
- File da scaricare e programmi si chiamano ora `Voltvale` (`Voltvale.exe`, `Voltvale.app`).

### Da sapere
- **Salvataggi**: la cartella ora si chiama «Voltvale». Al primo avvio i salvataggi delle versioni precedenti
  vengono **copiati** dalla cartella «Energy Grid Tycoon», che resta com'era.
- **Lingua**: la scelta fatta nel menu non passa alla versione nuova; al primo avvio vale di nuovo la lingua del
  sistema.
- L'indirizzo della versione web non cambia.
- Le traduzioni tedesca, francese e spagnola sono nuove: segnala pure le frasi strane.

### In English
- **New name and logo**: Voltvale, with «Energy Grid Tycoon» as the subtitle.
- **Three more languages**: German, French and Spanish, alongside Italian and English. On first launch the game
  uses your system language if it's one of the five.
- **Work**: about 56% of residents work. Power plants, solar and wind farms and mines need staff: with too few they
  produce less, with none they stop. Jobs go to energy first, then mines, then district services. Unemployment
  lowers taxes and a little happiness.
- **Night lights** on districts and the town hall, off when there's no power.
- Saves are **copied** from the old «Energy Grid Tycoon» folder on first launch; please pick your language again.

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
